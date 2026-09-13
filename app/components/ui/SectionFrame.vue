<script setup lang="ts">
withDefaults(defineProps<{
  id?: string
  tone?: 'dark' | 'light'
}>(), {
  tone: 'light'
})
</script>

<template>
  <section
    :id="id"
    class="section"
    :data-tone="tone"
    :class="tone === 'dark' ? 'bg-neutral-950 text-white' : 'bg-neutral-50 text-neutral-950'"
  >
    <div class="container-page py-24 md:py-32">
      <slot />
    </div>
  </section>
</template>
