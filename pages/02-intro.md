---
layout: center
---

# Scaling and Optimizing React Apps Isn't Easy

<div class="mt-12 flex items-center justify-center">
  <div v-click class="text-xl max-w-2xl text-center mb-12">
    Developers often rely on many external tools to manage builds, dependencies, and workflows.
  </div>
</div>

<div class="relative w-[600px] h-[400px] mx-auto">
  <!-- React Logo Center -->
  <div v-click class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
    <div class="w-32 h-32 bg-[#61DAFB]/10 rounded-full flex items-center justify-center z-10 relative">
      <i class="i-logos-react text-6xl"></i>
    </div>
  </div>
  
  <!-- Connection Lines -->
  <svg class="absolute inset-0 w-full h-full" style="z-index: 0;">
    <circle v-click class="connection-line" cx="50%" cy="50%" r="120" 
      stroke="currentColor" stroke-width="1" fill="none" 
      stroke-dasharray="4 4" opacity="0.2" />
  </svg>
  
  <!-- Tool Icons -->
  <div class="absolute w-full h-full">
    <!-- Webpack -->
    <div v-click class="absolute top-0 left-1/2 -translate-x-1/2 -translate-y-8">
      <div class="tool-icon">
        <i class="i-logos-webpack text-3xl"></i>
      </div>
      <div class="tool-label">Webpack</div>
    </div>
    <!-- Jest -->
    <div v-click class="absolute top-[25%] right-8 translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-jest text-3xl"></i>
      </div>
      <div class="tool-label">Jest</div>
    </div>
    <!-- Vite -->
    <div v-click class="absolute bottom-[25%] right-8 translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-vitejs text-3xl"></i>
      </div>
      <div class="tool-label">Vite</div>
    </div>
    <!-- ESLint -->
    <div v-click class="absolute bottom-0 left-1/2 -translate-x-1/2 translate-y-8">
      <div class="tool-icon">
        <i class="i-logos-eslint text-3xl"></i>
      </div>
      <div class="tool-label">ESLint</div>
    </div>
    <!-- Babel -->
    <div v-click class="absolute bottom-[25%] left-8 -translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-babel text-3xl"></i>
      </div>
      <div class="tool-label">Babel</div>
    </div>
    <!-- npm -->
    <div v-click class="absolute top-[25%] left-8 -translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-npm-icon text-3xl"></i>
      </div>
      <div class="tool-label">npm</div>
    </div>
  </div>
</div>

<style>
.tool-icon {
  @apply flex items-center justify-center mb-2 p-4 bg-gray-800/50 rounded-lg shadow-lg backdrop-blur-sm transition-transform duration-300;
}
.tool-icon:hover {
  @apply transform scale-110;
}
.tool-label {
  @apply text-sm text-gray-400 text-center whitespace-nowrap font-medium;
}
@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
.connection-line {
  animation: rotate 60s linear infinite;
}
</style>

<!--
React's ecosystem is vast and powerful, but it lacks a cohesive set of tools to manage complex applications efficiently.

That's where Nx steps in.
-->