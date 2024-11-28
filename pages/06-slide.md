---
layout: default
---

<div class="flex flex-col h-full">
  <!-- Header with gradient background -->
  <div class="text-center mb-8">
    <h1 class="text-4xl font-bold bg-gradient-to-r from-blue-500 to-purple-500 bg-clip-text text-transparent">
      Taking Your Project to the Next Level: Nx Cloud
    </h1>
  </div>

  <div class="flex-1 grid grid-cols-1 md:grid-cols-2 gap-12 px-8">
    <!-- Left Column: Visual Elements -->
    <div class="relative flex items-center justify-center">
      <!-- Central Cloud Icon -->
      <div v-click class="cloud-container">
        <i class="i-mdi-cloud text-6xl text-blue-400"></i>
      </div>
      <!-- React Logo -->
      <div v-click class="react-logo">
        <img 
          src="../images/react.png" 
          alt="React logo" 
          class="w-16 h-16 object-contain"
        />
      </div>
      <!-- Nx Logo -->
      <div v-click class="nx-logo">
        <img 
          src="../images/nx.png" 
          alt="Nx logo"
          class="w-12 h-12 object-contain"
        />
      </div>
      <!-- Connection Lines with Lightning Bolts -->
      <div v-click class="connection-lines">
        <i class="i-mdi-lightning-bolt text-yellow-400 bolt-1"></i>
        <i class="i-mdi-lightning-bolt text-yellow-400 bolt-2"></i>
        <i class="i-mdi-lightning-bolt text-yellow-400 bolt-3"></i>
      </div>
      <!-- Performance Indicators -->
      <div v-click class="performance-indicators">
        <div class="indicator speedometer">
          <i class="i-mdi-speedometer text-3xl text-green-400"></i>
        </div>
        <div class="indicator graph">
          <i class="i-mdi-trending-up text-3xl text-purple-400"></i>
        </div>
        <div class="indicator settings">
          <i class="i-mdi-cog text-3xl text-blue-400"></i>
        </div>
      </div>
    </div>
    <!-- Right Column: Benefits -->
    <div class="space-y-8">
      <div v-click class="benefit-card">
        <i class="i-mdi-rocket-launch text-3xl text-blue-400"></i>
        <div class="ml-4">
          <h3 class="text-xl font-bold mb-2">Built for Scale</h3>
        </div>
      </div>
      <div v-click class="benefit-card">
        <i class="i-mdi-flash text-3xl text-yellow-400"></i>
        <div class="ml-4">
          <h3 class="text-xl font-bold mb-2">Lightning Fast</h3>
        </div>
      </div>
      <div v-click class="benefit-card">
        <i class="i-mdi-chart-areaspline text-3xl text-green-400"></i>
        <div class="ml-4">
          <h3 class="text-xl font-bold mb-2">Intelligent Insights</h3>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
/* Container Styling */
.cloud-container {
  @apply relative p-8 bg-blue-500/10 rounded-full;
  animation: float 3s ease-in-out infinite;
}

/* React Logo */
.react-logo {
  @apply absolute -right-8 top-[30%] p-4 bg-[#61DAFB]/10 rounded-full;
  animation: spin 20s linear infinite;
}

/* Nx Logo */
.nx-logo {
  @apply absolute -left-8 top-[30%] p-4 bg-blue-500/10 rounded-full;
  animation: bounce 3s infinite;
}

/* Connection Lines */
.connection-lines {
  @apply absolute inset-0;
}
.bolt-1, .bolt-2, .bolt-3 {
  @apply absolute;
  animation: pulse 2s infinite;
}
.bolt-1 { top: 20%; right: 40%; animation-delay: 0s; }
.bolt-2 { top: 50%; right: 35%; animation-delay: 0.3s; }
.bolt-3 { top: 70%; right: 40%; animation-delay: 0.6s; }

/* Performance Indicators */
.performance-indicators {
  @apply absolute inset-0 pointer-events-none;
}
.indicator {
  @apply absolute p-3 bg-gray-800/50 rounded-full backdrop-blur-sm;
  animation: bounce 3s infinite;
}
.speedometer { top: 10%; left: 20%; animation-delay: 0s; }
.graph { top: 60%; left: 30%; animation-delay: 0.5s; }
.settings { top: 30%; left: 70%; animation-delay: 1s; }

/* Benefit Cards */
.benefit-card {
  @apply flex items-start p-6 bg-gray-800/50 rounded-xl backdrop-blur-sm
         border border-gray-700/50 transition-all duration-300;
}
.benefit-card:hover {
  @apply transform -translate-y-1 shadow-xl border-blue-500/30;
}

/* Animations */
@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}
@keyframes pulse {
  0%, 100% { opacity: 0.3; transform: scale(1); }
  50% { opacity: 1; transform: scale(1.2); }
}
@keyframes bounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-5px); }
}
@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
</style>
