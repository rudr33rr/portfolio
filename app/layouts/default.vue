<template>
  <div class="flex min-h-screen flex-col bg-neutral-950 text-white">
    <SiteHeader />
    <main class="flex-1">
      <slot />
    </main>
    <SiteFooter />
  </div>
</template>
