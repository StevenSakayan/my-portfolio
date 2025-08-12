<script setup>
  import Hero from './HeroSection.vue'
  import About from './AboutSection.vue'
  import Skills from './SkillsSection.vue'
  import Projects from './ProjectsSection.vue'
  import Education from './EducationSection.vue'

  import { onMounted } from 'vue'
import FooterComp from './FooterComp.vue'

  onMounted(() => {
    document.title = "Steven's Portfolio"
  })
</script>

<template>
  <div class="p-10 max-sm:p-6">
    <Hero />
    <About class="mx-auto my-20 max-w-2xl"/>
    <Skills class="mx-auto max-w-fit my-20"/>
    <Projects class="mx-auto my-20 max-w-fit"/>
    <Education class="mx-auto my-20 max-w-fit"/>
    <FooterComp />
  </div>
</template>

<style scoped>

</style>
