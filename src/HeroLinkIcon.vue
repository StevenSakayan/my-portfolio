<script setup>
  const props = defineProps({
    href: String,
  })
</script>

<template>
  <a class="w-10 h-10 flex shrink-0 justify-center items-center transition duration-200 ease-in-out hover:scale-110 fill-white" :href="props.href" target="_blank">
    <slot></slot>
  </a>
</template>
