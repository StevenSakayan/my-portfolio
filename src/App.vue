<script setup>
import Hero from './Hero.vue'
import About from './About.vue'
import Skills from './Skills.vue'
import Projects from './Projects.vue'
import Education from './Education.vue'

</script>

<template>
  <div class="p-10 max-sm:p-6">
    <Hero />
    <About class="mx-auto my-20 max-w-2xl"/>
    <Skills class="mx-auto max-w-fit my-20"/>
    <Projects class="mx-auto my-20 max-w-fit"/>
    <Education class="mx-auto my-20 max-w-fit"/>
  </div>
</template>

<style scoped>

</style>
