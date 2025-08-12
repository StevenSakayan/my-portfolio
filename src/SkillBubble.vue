<script setup>
	const props = defineProps({
		name: String,
		image: String,
	})

</script>

<template>
	<div class="w-40 h-auto max-sm:w-20">
		<div class="flex w-40 max-sm:w-20 h-40 max-sm:h-20 bg-white rounded-full items-center justify-center">
			<img class= "w-26 h-26 max-sm:w-15 max-sm:h-15 object-contain transition duration-200 ease-in-out hover:scale-110" :src="props.image"/>
		</div>
		<h2 class=" text-center font-bold pt-2">{{props.name}}</h2>
	</div>
</template>
