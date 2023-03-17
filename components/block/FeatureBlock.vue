<script setup lang="ts">
const { icon, title, description } = defineProps<{
  icon: string
  title: string
  description: string
  dark?: boolean
}>()
</script>

<template>
  <div
    class="w-[270px] h-[370px] shadow-2 text-white flex flex-column p-4"
    :class="dark ? 'bg-gray-600' : 'bg-yellow-600'"
  >
    <div class="flex flex-column justify-content-center align-items-center gap-4 text-center mt-15">
      <Image :src="icon" :alt="title" class="max-h-96px max-w-fit" />
      <h3>{{ title }}</h3>
    </div>
    <div class="flex gap-4 justify-content-center text-center mt-5">
      {{ description }}
    </div>
  </div>
</template>

<style scoped>

</style>
