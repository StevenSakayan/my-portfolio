<script setup>
    import downIcon from '@/icons/arrow-down.svg'
    import upIcon from '@/icons/arrow-up.svg'
    import closeIcon from '@/icons/close.svg'
    import WindowButton from './WindowButton.vue'
    const props = defineProps({
        title: String
    })
</script>

<template>
    <div class="rounded-md overflow-hidden">
        <div class="bg-slate-500 flex items-center relative">
            <h1 class="text-xl max-sm:text-lg mx-auto absolute left-0 right-0 w-fit text-center">{{ props.title }}</h1>
            <div class="ml-auto flex space-x-1 p-1">
                <WindowButton class="hover:bg-white active:bg-slate-400 ">
                    <downIcon class="group-hover:text-slate-500"/>
                </WindowButton>
                <WindowButton class="hover:bg-white active:bg-slate-400">
                    <upIcon class="group-hover:text-slate-500"/>
                </WindowButton>
                <WindowButton class="hover:bg-red-500 active:bg-red-700">
                    <closeIcon class="group-hover:text-slate-500"/>
                </WindowButton>
            </div>
        </div>
        <div class="bg-slate-800">
            <slot></slot>
        </div>
    </div>
</template>
