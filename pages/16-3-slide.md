---
layout: default
---

# Nx is Lightweight! 🪶

<div class="mt-8">
  <div class="grid grid-cols-2 gap-8">
    <!-- Left side: Key points -->
    <div v-click class="space-y-6">
      <div class="feature-card">
        <i class="i-mdi-clock-fast text-4xl text-green-500 mb-4" />
        <h3 class="font-bold text-lg mb-2">Quick Setup</h3>
        <div class="command-box mb-2">
          <span class="text-green-400">$</span> npx nx init
        </div>
        <p class="text-sm text-gray-400">Takes just seconds to run</p>
      </div>
      <div class="feature-card">
        <i class="i-mdi-feather text-4xl text-blue-500 mb-4" />
        <h3 class="font-bold text-lg mb-2">Minimal Changes</h3>
        <ul class="text-sm text-gray-400 list-disc list-inside space-y-2">
          <li>Adds only nx.json</li>
          <li>Minor package.json updates</li>
          <li>No code changes needed</li>
        </ul>
      </div>
    </div>
    <!-- Right side: Git diff visualization -->
    <div v-click class="flex flex-col">
      <div class="border dark:border-gray-700 rounded-lg p-4 h-full">
        <div class="text-center mb-4 font-bold">Git Diff omg</div>
        <div class="w-full h-[300px] bg-gray-100 dark:bg-gray-800 rounded flex items-center justify-center text-gray-400">
           <img 
      src="../images/gitdiff.png" 
      alt="Git diff visualization" 
    />
        </div>
      </div>
    </div>
  </div>
</div>

<style>
.feature-card {
  @apply p-6 rounded-lg border border-gray-200 dark:border-gray-700 
         transition-all duration-200 bg-gray-800/50 backdrop-blur-sm;
}

.feature-card:hover {
  @apply transform -translate-y-1 shadow-lg;
}

.command-box {
  @apply font-mono text-sm p-2 bg-gray-900/50 rounded;
}
</style>