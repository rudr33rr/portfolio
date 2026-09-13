<script setup lang="ts">
defineProps<{
  eyebrow?: string
  title: string
  description?: string
}>()
</script>

<template>
  <div class="mb-14 max-w-3xl">
    <p v-if="eyebrow" class="eyebrow mb-4">
      {{ eyebrow }}
    </p>
    <h2 class="text-4xl leading-[1.1] tracking-tight md:text-6xl">
      {{ title }}
    </h2>
    <p v-if="description" class="mt-5 max-w-xl text-lg leading-relaxed text-neutral-500">
      {{ description }}
    </p>
  </div>
</template>
