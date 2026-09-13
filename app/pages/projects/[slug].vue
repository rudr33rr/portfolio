<template>
  <SectionFrame tone="light">
    <NuxtLink to="/#work" class="mb-10 inline-block text-sm text-neutral-500 transition-colors hover:text-neutral-950">
      ← Wróć do projektów
    </NuxtLink>
    <SectionHeading
      eyebrow="Case study"
      :title="`Projekt: ${slug}`"
      description="Później: problem, Twoja rola, decyzje, wynik. Na start zostaje szkielet."
    />
    <div class="mb-4 aspect-21/9 rounded-2xl bg-neutral-100" />
    <div class="grid gap-4">
      <Placeholder label="Problem, który rozwiązywałem." />
      <Placeholder label="Co zrobiłem i dlaczego." />
      <Placeholder label="Efekt — liczba, cytat albo zrzut." />
    </div>
  </SectionFrame>
</template>

<script setup lang="ts">
const route = useRoute()
const slug = computed(() => String(route.params.slug))
</script>
