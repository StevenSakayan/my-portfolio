<script setup>
	const props = defineProps({
		name: String,
		image: String,
	});
</script>

<template>
	<div class="w-100 relative flex flex-col rounded-xl overflow-hidden flex-shrink-0 bg-slate-700 snap-center">
		<div class="aspect-video w-full">
			<img class="w-full h-full object-cover" :src="props.image"/>
		</div>
		<h2 class="text-2xl text-center pt-2">{{ name }}</h2>
		<div class="flex flex-1 px-4 pb-4 pt-2 items-center">
			<slot></slot>
		</div>
	</div>
</template>
