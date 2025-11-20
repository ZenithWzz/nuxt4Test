<template>
  <UCard class="mb-8">
    <template #header>
      <div class="flex items-center justify-between gap-4">
        <div>
          <p class="text-sm text-gray-500 dark:text-gray-400">Nuxt 4 + Nuxt UI</p>
          <h1 class="text-2xl font-semibold">Welcome to your Nuxt UI starter</h1>
        </div>
        <UIcon name="i-logos-nuxt" class="h-10 w-10" />
      </div>
    </template>
    <p>
      This starter is configured with Nuxt 4 and the Nuxt UI module so you can begin building a modern
      interface immediately.
    </p>
    <div class="mt-4 flex flex-wrap gap-3">
      <UButton to="https://nuxt.com/docs" target="_blank" icon="i-heroicons-book-open" color="primary" variant="solid">
        Nuxt Docs
      </UButton>
      <UButton to="https://ui.nuxt.com" target="_blank" icon="i-heroicons-sparkles" color="primary" variant="outline">
        Nuxt UI Docs
      </UButton>
    </div>
  </UCard>
</template>
