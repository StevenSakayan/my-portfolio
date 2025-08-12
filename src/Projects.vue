<script setup lang="ts">
import Window from './Window.vue';
import Project from './Project.vue';
</script>

<template>
	<Window title="Projects.pptx">
	    <div class="flex px-10 py-10 justify-center">
	      <div class="gap-5 flex flex-initial flex-row flex-nowrap overflow-x-auto scroll-smooth snap-x">
	        <Project name="Field Alert" image="./images/field-alert.png">
	          <ul class="list-disc list-inside">
	            <li>Web-based dashboard for custom agricultural alerts.</li>
	            <li>Integrating multiple data feeds through the Pairtree Pipes API.</li>
	            <li>Allows users to define alert conditions using live agtech data.</li>
	            <li>Alerts are displayed and sent via SMS, Email and WhatsApp.</li>
	          </ul>
	        </Project>
	        <Project name="Multiplayer Steam Game" image="./images/multiplayer-game.png">
	          <ul class="list-disc list-inside">
	            <li>Top-down randomly generated levels.</li>
	            <li>No port-forwarding required for multiplayer hosting.</li>
	            <li>Play on public lobbies or with Steam friends.</li>
	            <li>Created an efficient system to create, sync, and delete networked objects.</li>
	            <li>Sprite sheet system for custom player sprites.</li>
	          </ul>
	        </Project>
	        <Project name="Dolphini Config" image="./images/dolphini.png">
	          <ul class="list-disc list-inside">
	            <li>A tool designed for the Dolphin Emulator Software.</li>
	            <li>Creates config files that load for each emulated game.</li>
	            <li>Built all UI elements from the ground up, no framework or libraries.</li>
	          </ul>
	        </Project>
	      </div>
	    </div>
	</Window>
</template>
