---
layout: center
---

<div class="title-container">
  <h1>Scaling and Optimizing React Apps Isn't Easy</h1>
</div>

<div class="mt-8 flex flex-col items-center justify-center">
  <div class="text-xl max-w-2xl text-center mb-12">
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
  <svg class="absolute inset-0 w-full h-full">
    <circle v-click class="connection-line" cx="50%" cy="50%" r="120" 
      stroke="currentColor" stroke-width="1" fill="none" 
      stroke-dasharray="4 4" opacity="0.2" />
  </svg>
  
  <!-- Tool Icons -->
  <div class="absolute w-full h-full">
    <!-- Webpack -->
    <div v-click class="absolute top-4 left-1/2 -translate-x-1/2">
      <div class="tool-icon">
        <i class="i-logos-webpack text-3xl"></i>
      </div>
      <div class="tool-label">Webpack</div>
    </div>
    <!-- Jest -->
    <div v-click class="absolute top-[20%] right-6 translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-jest text-3xl"></i>
      </div>
      <div class="tool-label">Jest</div>
    </div>
    <!-- Vite -->
    <div v-click class="absolute bottom-[20%] right-6 translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-vitejs text-3xl"></i>
      </div>
      <div class="tool-label">Vite</div>
    </div>
    <!-- ESLint -->
    <div v-click class="absolute bottom-8 left-1/2 -translate-x-1/2">
      <div class="tool-icon">
        <i class="i-logos-eslint text-3xl"></i>
      </div>
      <div class="tool-label">ESLint</div>
    </div>
    <!-- Babel -->
    <div v-click class="absolute bottom-[20%] left-6 -translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-babel text-3xl"></i>
      </div>
      <div class="tool-label">Babel</div>
    </div>
    <!-- npm -->
    <div v-click class="absolute top-[20%] left-6 -translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-npm-icon text-3xl"></i>
      </div>
      <div class="tool-label">npm</div>
    </div>
  </div>
</div>

<style>
/* Title styling to avoid cutoff */
.title-container {
  text-align: center;
  margin-top: 2rem; /* Adjust for screen padding */
}
.title-container h1 {
  font-size: 2rem; /* Scales nicely for all screens */
  line-height: 1;
  margin: 0 auto;
}

/* Tool icon styles */
.tool-icon {
  @apply flex items-center justify-center mb-2 p-4 bg-gray-800/50 rounded-lg shadow-lg backdrop-blur-sm transition-transform duration-300;
}
.tool-icon:hover {
  @apply transform scale-110;
}
.tool-label {
  @apply text-sm text-gray-400 text-center whitespace-nowrap font-medium;
}

/* Circle animation stays static */
@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
.connection-line {
  animation: rotate 30s linear infinite; /* Smooth rotation in place */
  transform-origin: center; /* Ensures the circle stays centered */
  r: 120; /* Fixed radius */
}
</style>
