<script setup lang="ts">
const props = defineProps<{
  to: string
}>()
</script>

<template>
  <NuxtLink :to="props.to" target="_blank" class="text-stone-700 decoration-pink-200 hover:decoration-pink-400 hover:text-stone-900 underline inline-flex underline-offset-2">
    <slot />
  </NuxtLink>
</template>
