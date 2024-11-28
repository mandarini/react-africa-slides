---
layout: default
---

<div class="title-container">
  <h1>Code Generators That Save Time</h1>
</div>

<div class="flex flex-col items-center mt-4">
  <div v-click class="text-xl text-center max-w-3xl mb-6">
    Speed up development with powerful generators
  </div>
</div>

<!-- Top Row: Applications and Libraries -->
<div class="grid grid-cols-2 gap-6 px-6 mb-6">
  <div v-click class="generator-card">
    <div class="flex items-center gap-3 mb-3">
      <i class="i-mdi-application text-2xl text-blue-400"></i>
      <h3 class="text-lg font-bold">Applications</h3>
    </div>
    <div class="command-box">
      <span class="text-green-400">$</span> nx g @nx/react:app my-app
    </div>
  </div>
  <div v-click class="generator-card">
    <div class="flex items-center gap-3 mb-3">
      <i class="i-mdi-library text-2xl text-purple-400"></i>
      <h3 class="text-lg font-bold">Libraries</h3>
    </div>
    <div class="command-box">
      <span class="text-green-400">$</span> nx g @nx/react:lib shared-ui
    </div>
  </div>
</div>

<!-- Middle Row: Components and Hooks -->
<div class="grid grid-cols-2 gap-6 px-6 mb-8">
  <div v-click class="generator-card">
    <div class="flex items-center gap-3 mb-3">
      <i class="i-mdi-puzzle text-2xl text-teal-400"></i>
      <h3 class="text-lg font-bold">Components</h3>
    </div>
    <div class="command-box">
      <span class="text-green-400">$</span> nx g @nx/react:component button
    </div>
  </div>
  <div v-click class="generator-card">
    <div class="flex items-center gap-3 mb-3">
      <i class="i-mdi-hook text-2xl text-amber-400"></i>
      <h3 class="text-lg font-bold">Hooks</h3>
    </div>
    <div class="command-box">
      <span class="text-green-400">$</span> nx g @nx/react:hook use-auth
    </div>
  </div>
</div>

<!-- Bottom: Flow Diagram -->
<div v-click class="px-6">
  <div class="flow-diagram">
    <div class="flow-step">
      <i class="i-mdi-code-braces text-2xl text-blue-400"></i>
      <span>Generate</span>
    </div>
    <div class="flow-arrow">
      <i class="i-mdi-arrow-right text-lg"></i>
    </div>
    <div class="flow-step">
      <i class="i-mdi-cog text-2xl text-purple-400"></i>
      <span>Build</span>
    </div>
    <div class="flow-arrow">
      <i class="i-mdi-arrow-right text-lg"></i>
    </div>
    <div class="flow-step">
      <i class="i-mdi-test-tube text-2xl text-teal-400"></i>
      <span>Test</span>
    </div>
    <div class="flow-arrow">
      <i class="i-mdi-arrow-right text-lg"></i>
    </div>
    <div class="flow-step">
      <i class="i-mdi-rocket-launch text-2xl text-amber-400"></i>
      <span>Deploy</span>
    </div>
  </div>
</div>

<style>
.title-container {
  text-align: center;
  margin-top: 1rem;
}

.generator-card {
  @apply bg-gray-800/50 backdrop-blur-sm p-4 rounded-xl border border-gray-700/50 
         transition-all duration-300 hover:transform hover:-translate-y-1 hover:shadow-lg;
}

.command-box {
  @apply bg-gray-900/50 p-2 rounded font-mono text-sm;
}

.command-box:hover {
  @apply bg-gray-900/80;
}

.flow-diagram {
  @apply flex items-center justify-center gap-4 bg-gray-800/30 p-4 rounded-xl backdrop-blur-sm
         border border-gray-700/30;
}

.flow-step {
  @apply flex flex-col items-center gap-1 p-2 bg-gray-800/50 rounded-lg
         transition-all duration-300 hover:transform hover:scale-105;
}

.flow-step span {
  @apply text-xs text-gray-400 font-medium;
}

.flow-arrow {
  @apply text-gray-500;
}
</style>