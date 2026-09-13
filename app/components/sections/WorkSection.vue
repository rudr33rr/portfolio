<template>
  <SectionFrame id="work" tone="light">
    <SectionHeading
      eyebrow="Wybrane realizacje"
      title="Projekty, które to potwierdzają"
      description="2–3 case studies. Klik otworzy osobną stronę projektu."
    />
    <div class="grid gap-4 md:grid-cols-3">
      <NuxtLink
        v-for="project in projects"
        :key="project.slug"
        :to="`/projects/${project.slug}`"
        class="card group block p-0"
      >
        <div class="aspect-[16/10] bg-neutral-100" />
        <div class="p-6">
          <p class="eyebrow mb-3">Case study</p>
          <p class="text-lg leading-snug">{{ project.label }}</p>
        </div>
      </NuxtLink>
    </div>
  </SectionFrame>
</template>

<script setup lang="ts">
const projects = [
  { slug: 'projekt-1', label: 'Projekt 1 — problem, rola, wynik.' },
  { slug: 'projekt-2', label: 'Projekt 2 — problem, rola, wynik.' },
]
</script>
