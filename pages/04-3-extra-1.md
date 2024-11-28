---
layout: default
---

<div class="title-container">
  <h1>Streamline Development with Nx</h1>
</div>

<div class="grid grid-cols-3 gap-8 mt-12 px-4">
  <!-- Testing Section -->
  <div v-click class="feature-section">
    <div class="icon-wrapper">
      <div class="flex gap-2">
        <i class="i-logos-jest text-3xl"></i>
        <i class="i-logos-cypress text-3xl"></i>
      </div>
    </div>
    <h3 class="text-xl font-bold mt-4 mb-2">Testing Made Simple</h3>
    <div class="command-box">
      <span class="text-green-400">$</span> nx test
    </div>
    <div class="command-box mt-2">
      <span class="text-green-400">$</span> nx e2e
    </div>
    <p class="text-sm text-gray-400 mt-4">
      Seamless Jest and Cypress integration for unit and E2E testing
    </p>
  </div>

  <!-- Build Section -->
  <div v-click class="feature-section">
    <div class="icon-wrapper">
      <i class="i-mdi-package-variant-closed text-4xl"></i>
    </div>
    <h3 class="text-xl font-bold mt-4 mb-2">Optimized Builds</h3>
    <div class="command-box">
      <span class="text-green-400">$</span> nx build
    </div>
    <div class="command-box mt-2">
      <span class="text-green-400">$</span> nx release
    </div>
    <p class="text-sm text-gray-400 mt-4">
      Build deployable apps or publishable libraries with ease
    </p>
  </div>

  <!-- SSR & Module Federation -->
  <div v-click class="feature-section">
    <div class="icon-wrapper">
      <i class="i-mdi-server-network text-4xl"></i>
    </div>
    <h3 class="text-xl font-bold mt-4 mb-2">SSR & Module Federation</h3>
    <div class="command-box">
      <span class="text-green-400">$</span>nx g @nx/react:setup-ssr
    </div>
    <div class="command-box mt-2">
      <span class="text-green-400">$</span>nx serve host-app
    </div>
    <div class="command-box mt-2">
      <span class="text-green-400">$</span>nx g @nx/react:remote
    </div>
    <p class="text-sm text-gray-400 mt-4">
      Generate SSR apps and federate modules effortlessly
    </p>
  </div>
</div>

<style>
.title-container {
  text-align: center;
  margin-top: 2rem;
}

.feature-section {
  @apply bg-gray-800/50 backdrop-blur-sm p-6 rounded-xl border border-gray-700/50 
         transition-all duration-300 hover:transform hover:-translate-y-1 hover:shadow-xl;
}

.icon-wrapper {
  @apply w-16 h-16 rounded-full flex items-center justify-center mb-4 mx-auto
         bg-blue-500/10 transition-transform duration-300;
}

.feature-section:hover .icon-wrapper {
  @apply transform scale-110;
}

.command-box {
  @apply bg-gray-900/50 p-2 rounded font-mono text-sm mt-2;
}

.command-box:hover {
  @apply bg-gray-900/80;
}
</style>