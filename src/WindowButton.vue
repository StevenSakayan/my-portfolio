<template>
	<button class="btn btn-circle btn-sm bg-transparent shadow-none border-0 active:translate-0 group">
		<slot></slot>
	</button>
</template>

<style>
	 button:active {
		translate: 0 0;
	 }
</style>