---
layout: center
---

<div class="title-container">
  <h1>Nx: The Missing Piece for React Developers</h1>
</div>

<div class="mt-8 flex flex-col items-center justify-center">
  <div class="text-xl max-w-2xl text-center mb-12">
    Nx brings cohesion to the React ecosystem, simplifying development with powerful automation and tooling integration.
  </div>
</div>

<div class="relative w-[600px] h-[400px] mx-auto">
  <!-- Nx Logo Center -->
  <div v-click class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
    <div class="w-32 h-32 bg-blue-500/10 rounded-full flex items-center justify-center z-10 relative">
      <img 
        src="../images/nx.png" 
        alt="Nx logo"
        class="w-20 h-20 object-contain"
      />
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
    <!-- React -->
    <div v-click class="absolute top-4 left-1/2 -translate-x-1/2">
      <div class="tool-icon">
        <i class="i-logos-react text-3xl"></i>
      </div>
      <div class="tool-label">React</div>
    </div>
    <!-- Vite -->
    <div v-click class="absolute top-[20%] right-6 translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-vitejs text-3xl"></i>
      </div>
      <div class="tool-label">Vite</div>
    </div>
    <!-- Vitest -->
    <div v-click class="absolute bottom-[20%] right-6 translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-vitest text-3xl"></i>
      </div>
      <div class="tool-label">Vitest</div>
    </div>
    <!-- Next.js -->
    <div v-click class="absolute bottom-8 left-1/2 -translate-x-1/2">
      <div class="tool-icon">
        <i class="i-logos-nextjs-icon text-3xl"></i>
      </div>
      <div class="tool-label">Next.js</div>
    </div>
    <!-- Playwright -->
    <div v-click class="absolute bottom-[20%] left-6 -translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-playwright text-3xl"></i>
      </div>
      <div class="tool-label">Playwright</div>
    </div>
    <!-- Remix -->
    <div v-click class="absolute top-[20%] left-6 -translate-x-8">
      <div class="tool-icon">
        <i class="i-logos-remix-icon text-3xl"></i>
      </div>
      <div class="tool-label">Remix</div>
    </div>
  </div>
</div>

<style>
/* Title styling to avoid cutoff */
.title-container {
  text-align: center;
  margin-top: 2rem;
}
.title-container h1 {
  font-size: 2rem;
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
  animation: rotate 30s linear infinite;
  transform-origin: center;
  r: 120;
}
</style>

<!--
Nx acts as the glue for the React ecosystem, offering an integrated approach to managing your app.
With built-in code generators and automated migrations, Nx saves you from tedious manual steps and accelerates your development process.
-->