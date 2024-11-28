---
layout: default
---

<div class="title-container">
  <h1 class="text-4xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-blue-500 to-purple-500">
    Nx Supercharges React Development
  </h1>
</div>

<div class="flex flex-col h-full items-center">
  <!-- React Logo at Top -->
  <div class="flex justify-center items-center h-48 relative">
    <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
      <div class="w-32 h-32 bg-[#61DAFB]/10 rounded-full flex items-center justify-center">
        <i class="i-logos-react text-6xl animate-spin-slow"></i>
      </div>
    </div>
  </div>

  <!-- Connecting Lines Container -->
  <div class="flex-1 relative w-full max-w-4xl">
    <svg class="absolute inset-0 w-full h-full" viewBox="0 0 800 400" preserveAspectRatio="xMidYMid meet">
      <g class="connections">
        <path v-click class="connection-line" d="M400,100 L100,300" />
        <path v-click class="connection-line" d="M400,100 L300,300" />
        <path v-click class="connection-line" d="M400,100 L500,300" />
        <path v-click class="connection-line" d="M400,100 L600,300" />
        <path v-click class="connection-line" d="M400,100 L700,300" />
      </g>
    </svg>
  </div>

  <!-- Tools Row at Bottom -->
  <div class="w-full max-w-4xl grid grid-cols-5 gap-8 px-12 mb-12">
    <div v-click class="tool-container">
      <i class="i-logos-nextjs-icon text-4xl"></i>
      <span class="tool-label">Next.js</span>
    </div>
    <div v-click class="tool-container">
      <i class="i-logos-remix-icon text-4xl"></i>
      <span class="tool-label">Remix</span>
    </div>
    <div v-click class="tool-container">
      <i class="i-logos-vitejs text-4xl"></i>
      <span class="tool-label">Vite</span>
    </div>
    <div v-click class="tool-container">
      <div class="flex gap-2">
        <i class="i-logos-jest text-4xl"></i>
        <i class="i-logos-vitest text-4xl"></i>
      </div>
      <span class="tool-label">Jest & Vitest</span>
    </div>
    <div v-click class="tool-container">
      <i class="i-logos-playwright text-4xl"></i>
      <span class="tool-label">Playwright</span>
    </div>
  </div>
</div>

<style>
.animate-spin-slow {
  animation: spin 20s linear infinite;
}

@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.tool-container {
  @apply flex flex-col items-center gap-2 p-4 rounded-lg transition-all duration-300
         bg-gray-800/50 backdrop-blur-sm hover:transform hover:scale-110;
}

.tool-label {
  @apply text-sm text-gray-400 font-medium;
}

.connection-line {
  fill: none;
  stroke: rgba(255, 255, 255, 0.1);
  stroke-width: 2;
  stroke-dasharray: 10;
  animation: flow 2s linear infinite;
}

@keyframes flow {
  from {
    stroke-dashoffset: 20;
  }
  to {
    stroke-dashoffset: 0;
  }
}
</style>