<script setup>
	const props = defineProps({
		name: String,
		image: String,
	})

</script>

<template>
	<div class="w-40 h-auto">
		<div class="flex w-40 h-40 bg-white rounded-full items-center justify-center">
			<img class= "w-26 h-26 object-contain transition duration-200 ease-in-out hover:scale-110" :src="props.image"></img>
		</div>
		<h2 class="text-center font-bold p-3">{{props.name}}</h2>
	</div>
</template>
