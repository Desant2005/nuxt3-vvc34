<script setup lang="ts">
import FeatureBlock from '~/components/block/FeatureBlock.vue'

const features = computed(() => {
  return [
    {
      title: 'Более 6 лет с вами',
      description: 'Высококвалифицированные специалисты широкого и узкого профиля.',
      icon: 'features/feature-1.png',
      dark: true,
    },
    {
      title: 'Оборудование',
      description: 'Современные методы УЗ-диагностики и лобораторных исследований.',
      icon: 'features/feature-2.png',
      dark: false,
    },
    {
      title: 'Доверие клиентов',
      description: '85% наших клиентов обращаются к нам повторно.',
      icon: 'features/feature-3.png',
      dark: true,
    },
    {
      title: 'Хирургия XXI',
      description: 'Проведение хирургических операций любой категории сложности.',
      icon: 'features/feature-4.png',
      dark: false,
    },
  ]
})
</script>

<template>
  <div class="flex gap-4 justify-content-center">
    <FeatureBlock
      v-for="feature in features" :key="feature.title"
      :title="feature.title"
      :icon="feature.icon"
      :description="feature.description"
      :dark="feature.dark"
    />
  </div>
</template>
