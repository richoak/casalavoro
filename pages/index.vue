<template>
  <main>
    <hero-section />
    <hero-feature />
    <feature-one />
    <feature-two />
    <feature-three />
    <feature-four />
    <stat-section />
    <!-- <testimonial-section /> -->
    <updated-testimonials />
    <cta-section />
    <frequently-asked-questions />
    <contact-map />
    <contact-section />
    <footer-section />
  </main>
</template>

<script setup lang="ts">
const productName: string = "Nuxt 3 Starter Kit";
const features: string[] = ["Vite", "Vue 3", "TypeScript", "PostCSS", "TailwindCSS"];
const message = computed(
  () => `This is a ${productName} with ${features.slice(0, -1).join(", ")} and ${features.slice(-1)}!`
);

definePageMeta({
  layout: false,
});
</script>