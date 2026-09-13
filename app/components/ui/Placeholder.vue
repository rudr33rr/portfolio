<script setup lang="ts">
defineProps<{
  label: string
}>()
</script>

<template>
  <div class="card h-full">
    <p class="text-base leading-relaxed text-neutral-500">{{ label }}</p>
    <slot />
  </div>
</template>
