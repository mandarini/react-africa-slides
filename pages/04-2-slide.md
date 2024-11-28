---
layout: default
---

<div class="title-container">
  <h1 class="text-4xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-blue-500 to-purple-500">
    Nx Supercharges React Development
  </h1>
</div>

<div class="relative w-[700px] h-[500px] mx-auto mt-8">
  <!-- React Logo Center -->
  <div v-click class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
    <div class="w-32 h-32 bg-[#61DAFB]/10 rounded-full flex items-center justify-center z-10 relative">
      <i class="i-logos-react text-6xl animate-spin-slow"></i>
    </div>
  </div>
  
  <!-- Connection Lines -->
  <svg class="absolute inset-0 w-full h-full">
    <circle v-click class="connection-line" cx="50%" cy="50%" r="150" 
      stroke="currentColor" stroke-width="1" fill="none" 
      stroke-dasharray="4 4" opacity="0.2" />
  </svg>
  
  <!-- Tool Icons -->
  <div class="absolute w-full h-full">
    <!-- Next.js -->
    <div v-click class="absolute top-0 left-1/2 -translate-x-1/2">
      <div class="tool-icon">
        <i class="i-logos-nextjs-icon text-3xl"></i>
      </div>
      <div class="tool-label">Next.js</div>
    </div>
    <!-- Remix -->
    <div v-click class="absolute top-[15%] right-[10%]">
      <div class="tool-icon">
        <i class="i-logos-remix-icon text-3xl"></i>
      </div>
      <div class="tool-label">Remix</div>
    </div>
    <!-- Vite -->
    <div v-click class="absolute top-[65%] right-[10%]">
      <div class="tool-icon">
        <i class="i-logos-vitejs text-3xl"></i>
      </div>
      <div class="tool-label">Vite</div>
    </div>
    <!-- Jest -->
    <div v-click class="absolute bottom-0 right-[30%]">
      <div class="tool-icon">
        <i class="i-logos-jest text-3xl"></i>
      </div>
      <div class="tool-label">Jest</div>
    </div>
    <!-- Vitest -->
    <div v-click class="absolute bottom-0 left-[30%]">
      <div class="tool-icon">
        <i class="i-logos-vitest text-3xl"></i>
      </div>
      <div class="tool-label">Vitest</div>
    </div>
    <!-- Playwright -->
    <div v-click class="absolute top-[65%] left-[10%]">
      <div class="tool-icon">
        <i class="i-logos-playwright text-3xl"></i>
      </div>
      <div class="tool-label">Playwright</div>
    </div>
    <!-- Module Federation -->
    <div v-click class="absolute top-[15%] left-[10%]">
      <div class="tool-icon">
        <i class="i-logos-webpack text-3xl"></i>
      </div>
      <div class="tool-label">Module Federation</div>
    </div>
  </div>
</div>

<style>
.title-container {
  text-align: center;
  margin-top: 2rem;
}

.tool-icon {
  @apply flex items-center justify-center mb-2 p-4 bg-gray-800/50 rounded-lg 
         shadow-lg backdrop-blur-sm transition-all duration-300 border border-gray-700/30;
}

.tool-icon:hover {
  @apply transform scale-110 border-blue-500/50 bg-gray-800/80;
  box-shadow: 0 0 20px rgba(59, 130, 246, 0.2);
}

.tool-label {
  @apply text-sm text-gray-400 text-center whitespace-nowrap font-medium;
}

@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.connection-line {
  animation: rotate 30s linear infinite;
  transform-origin: center;
}

.animate-spin-slow {
  animation: spin 20s linear infinite;
}

@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
</style>