---
layout: default
---

# What's New for Angular in Nx

<div class="grid grid-cols-2 gap-8 mt-12">
  <div v-click class="feature-update">
    <i class="i-mdi-test-tube text-3xl text-green-500" />
    <h3 class="text-xl font-semibold mt-2">Vitest Support</h3>
    <p class="text-sm text-gray-600 dark:text-gray-400">Unit testing for Angular apps</p>
  </div>

  <div v-click class="feature-update">
    <i class="i-mdi-angular text-3xl text-red-500" />
    <h3 class="text-xl font-semibold mt-2">Angular 19</h3>
    <p class="text-sm text-gray-600 dark:text-gray-400">Full support</p>
  </div>

  <div v-click class="feature-update">
    <i class="i-mdi-rocket-launch text-3xl text-purple-500" />
    <h3 class="text-xl font-semibold mt-2">Rspack Support</h3>
    <p class="text-sm text-gray-600 dark:text-gray-400">Experimental</p>
  </div>

  <div v-click class="feature-update">
    <i class="i-mdi-cube-scan text-3xl text-blue-500" />
    <h3 class="text-xl font-semibold mt-2">Module Federation Generators</h3>
    <p class="text-sm text-gray-600 dark:text-gray-400">Ongoing investment</p>
  </div>
</div>

<div class="absolute bottom-4 left-0 right-0 text-gray-400 text-sm text-center">
  @psybercity - @NxDevTools - 🦋 @psyber.city - 🦋 @nx.dev - Katerina Skroumpelou - AngularDay2024
</div>

<style>
.feature-update {
  @apply p-6 rounded-xl border border-gray-200 dark:border-gray-700 text-center transition-all duration-200;
}
.feature-update:hover {
  @apply shadow-lg transform -translate-y-1;
}
</style>