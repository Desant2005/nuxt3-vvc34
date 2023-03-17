<script setup>
const title = ref('layout home')
</script>

<template>
  <main class="py-20 px-10 text-center">
    <h1>{{ title }}</h1>
    <slot />
  </main>
</template>
