<script setup>
    import {ref, onMounted, onBeforeUnmount} from 'vue';
    const props = defineProps({
        text: {
            type: String
        },
        speed: {
            type: Number,
            default: 300,
        }
    })

    const output = ref('');
    const binOutput = ref('');
    let currentLetterIndex = 0;
    let currentBitIndex = 0;
    let intervalId = null;

    function toBinary(char) {
        return char.charCodeAt(0).toString(2).padStart(8,'0');
    }

    function typeNextLetter() {
        const letter = props.text[currentLetterIndex];
        const binary = toBinary(letter);
        currentBitIndex = 0;

        intervalId = setInterval(() => {
            if (currentBitIndex < binary.length) {
                binOutput.value += binary[currentBitIndex];
                currentBitIndex++;
            } else {
                clearInterval(intervalId);
                output.value += letter;
                binOutput.value = '';

                currentLetterIndex++;
                if (currentLetterIndex != props.text.length) {
                    setTimeout(() => {
                        typeNextLetter();
                    }, 50);
                }
            }
        }, props.speed);
    }

    onMounted(() => {
        output.value = '';
        binOutput.value = '';
        currentLetterIndex = 0;
        currentBitIndex = 0;
        typeNextLetter();
    });

    onBeforeUnmount(() => {
        clearInterval(intervalId);
    });
</script>

<template>
    <div>
        <div class="inline-block">{{output}}</div>
        <div class="inline-block text-slate-500 text-xl font-medium pl-2">{{binOutput}}</div>
    </div>
</template>
