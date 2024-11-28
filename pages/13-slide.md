---
layout: default
---

# What's New in the Nx Cloud App

<div class="mt-12">
  <div class="grid grid-cols-3 gap-6">
    <div v-click class="feature-card">
      <i class="i-mdi-download text-4xl text-blue-500" />
      <h3 class="font-bold mt-4">Download Task Artifacts</h3>
      <p class="text-sm mt-2">Access task outputs directly</p>
    </div>
    <div v-click class="feature-card">
      <i class="i-mdi-shield-key text-4xl text-green-500" />
      <h3 class="font-bold mt-4">Improved Access Control</h3>
      <p class="text-sm mt-2">Personal Access Tokens, nx-cloud login</p>
    </div>
    <div v-click class="feature-card">
      <i class="i-mdi-graph text-4xl text-purple-500" />
      <h3 class="font-bold mt-4">CIPE Affected Project Graph</h3>
      <p class="text-sm mt-2">Visualize impacted projects in CI</p>
    </div>
  </div>
</div>

<div class="absolute bottom-4 left-0 right-0 text-gray-400 text-sm text-center">
  @psybercity - @NxDevTools - 🦋 @psyber.city - 🦋 @nx.dev - Katerina Skroumpelou - React Africa 2024
</div>

<style>
.feature-card {
  @apply p-6 rounded-lg border border-gray-200 dark:border-gray-700 text-center transition-all duration-200;
}
.feature-card:hover {
  @apply shadow-lg transform -translate-y-1;
}
</style>