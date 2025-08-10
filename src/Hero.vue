<script setup lang="ts">
import BinaryTyper from './BinaryTyper.vue';
import Window from './Window.vue';

</script>

<template>
	<div class="h-screen flex items-center justify-center">
		<Window class="" title="Hello World.cmd">
			<div class="flex items-center h-auto gap-2 p-10">
				<div class="">
					<BinaryTyper text="Hello World!" :speed="30" class="w-80 text-left text-3xl font-bold"></BinaryTyper>
					<h2 class="text-2xl">Welcome to my Portfolio!</h2>
				</div>
				<div class="divider divider-horizontal"></div>
				<div class="items-center text-center"> 
					<div class="avatar py-4">
					<div class="w-64 rounded-full ring-3 ring-emerald-300">
						<img src="/images/me.jpeg"/>
					</div>
					</div>
					<h2 class="text-3xl font-bold">Steven Sakayan</h2>
					<h2 class="text-2xl">Software Developer</h2>
				</div>
			</div>
		</Window>
	  </div>
</template>
