<script lang="ts" setup>
const props = withDefaults(defineProps<{
  to: string
  icon?: string
  target?: string
}>(), {
  icon: 'fa-solid:rocket',
  target: '_self',
})
</script>

<template>
  <NuxtLink :to="props.to" :target="props.target" class="flex items-center p-5 px-10 gap-x-4 bg-slate-50 hover:bg-pink-50 group">
    <div class="text-3xl text-stone-300 flex items-center group-hover:text-pink-400">
      <Icon :name="props.icon" />
    </div>
    <span class="text-stone-500 group-hover:text-pink-700">
      <slot />
    </span>
  </NuxtLink>
</template>
