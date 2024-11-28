---
layout: default
---

# Distributed Task Execution (Nx Agents)

<div class="mt-12">
  <div v-click class="text-xl mb-8">
    Speed up CI builds with Nx Agents distributing tasks.
  </div>

  <div class="grid grid-cols-3 gap-6">
    <div v-click class="agent-card">
      <i class="i-mdi-server text-4xl text-purple-500" />
      <div class="text-lg font-bold mt-2">Agent 1</div>
      <div class="text-sm">Unit Tests</div>
    </div>
    <div v-click class="agent-card">
      <i class="i-mdi-server text-4xl text-blue-500" />
      <div class="text-lg font-bold mt-2">Agent 2</div>
      <div class="text-sm">Build Tasks</div>
    </div>
    <div v-click class="agent-card">
      <i class="i-mdi-server text-4xl text-green-500" />
      <div class="text-lg font-bold mt-2">Agent 3</div>
      <div class="text-sm">E2E Tests</div>
    </div>
  </div>

  <div v-click class="mt-8 text-center text-gray-500">
    Tasks are intelligently distributed across available agents
  </div>
</div>

<div class="absolute bottom-4 left-0 right-0 text-gray-400 text-sm text-center">
  @psybercity - @NxDevTools - 🦋 @psyber.city - 🦋 @nx.dev - Katerina Skroumpelou - AngularDay2024
</div>

<style>
.agent-card {
  @apply p-6 rounded-lg border border-gray-200 dark:border-gray-700 text-center transition-all duration-200;
}
.agent-card:hover {
  @apply shadow-lg transform -translate-y-1;
}
</style>