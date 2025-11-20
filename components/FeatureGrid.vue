<template>
  <div class="grid gap-6 md:grid-cols-2 xl:grid-cols-3">
    <UCard v-for="feature in features" :key="feature.title">
      <template #header>
        <div class="flex items-center gap-3">
          <UIcon :name="feature.icon" class="h-6 w-6 text-primary-500" />
          <div>
            <p class="text-sm text-gray-500 dark:text-gray-400">{{ feature.tagline }}</p>
            <h2 class="text-xl font-medium">{{ feature.title }}</h2>
          </div>
        </div>
      </template>
      <p class="text-gray-700 dark:text-gray-200">{{ feature.description }}</p>
    </UCard>
  </div>
</template>

<script setup lang="ts">
const features = [
  {
    title: 'Vue 3 & Nuxt 4',
    tagline: 'Composition API ready',
    description: 'Build with the latest Nuxt 4 runtime powered by Vue 3 and Vite.',
    icon: 'i-logos-nuxt-icon'
  },
  {
    title: 'Nuxt UI built-in',
    tagline: 'Design system',
    description: 'Access UI components, icons, and composables without extra setup.',
    icon: 'i-heroicons-sparkles'
  },
  {
    title: 'TypeScript support',
    tagline: 'Strict typing',
    description: 'Leverage Nuxt typings and auto-imports for a smooth developer experience.',
    icon: 'i-heroicons-command-line'
  },
  {
    title: 'Best practices',
    tagline: 'Conventions first',
    description: 'Enjoy file-based routing, auto-imports, and server routes out of the box.',
    icon: 'i-heroicons-check-badge'
  },
  {
    title: 'Production ready',
    tagline: 'Optimized builds',
    description: 'Generate static or server builds with Nitro-powered rendering.',
    icon: 'i-heroicons-rocket-launch'
  },
  {
    title: 'Extendable',
    tagline: 'Modules ecosystem',
    description: 'Add modules like content, auth, or i18n through the Nuxt module system.',
    icon: 'i-heroicons-puzzle-piece'
  }
];
</script>
