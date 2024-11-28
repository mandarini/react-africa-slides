---
layout: default
---

# Atomizer: E2E Test Optimization

<div class="mt-12">
  <div v-click class="text-xl mb-8">
    Automatically split and parallelize E2E tests.
  </div>

  <div class="grid grid-cols-2 gap-8">
    <div v-click class="space-y-6">
      <div class="bg-purple-50 dark:bg-purple-900 p-6 rounded-lg">
        <h3 class="font-bold text-lg mb-4">
          <i class="i-mdi-atom mr-2" />
          Smart Test Distribution
        </h3>
        <ul class="list-disc ml-4 space-y-2">
          <li>Automatic test splitting</li>
          <li>Parallel execution</li>
          <li>Optimal resource usage</li>
        </ul>
      </div>
    </div>
    <div v-click class="flex items-center justify-center">
      <div class="relative w-full">
        <div class="space-y-4">
          <div class="text-sm font-mono opacity-50 mb-6">Original Test Files:</div>
          <div v-for="n in 4" :key="`orig-${n}`" class="test-block">
            src/e2e/app{{ n }}.cy.ts
          </div>
          <div class="text-sm font-mono opacity-50 my-6">Atomizer Split:</div>
          <div v-for="n in 4" :key="`split-${n}`" class="test-block split" :style="{ animationDelay: `${n * 0.2}s` }">
            e2e-ci--src/e2e/app{{ n }}.cy.ts
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="absolute bottom-4 left-0 right-0 text-gray-400 text-sm text-center">
  @psybercity - @NxDevTools - 🦋 @psyber.city - 🦋 @nx.dev - Katerina Skroumpelou - React Africa 2024
</div>
</div>

<style>
.test-block {
  @apply p-2 text-sm font-mono rounded;
  @apply bg-gray-100 dark:bg-gray-800;
}

.test-block.split {
  @apply bg-blue-50 dark:bg-blue-900;
  animation: slideIn 0.5s ease-out forwards;
  opacity: 0;
  transform: translateY(20px);
}

@keyframes slideIn {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
