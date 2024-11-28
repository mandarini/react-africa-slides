---
layout: default
---

# Remote Caching (Nx Replay)

<div class="mt-8">
  <div v-click class="text-xl text-center mb-8">
    Accelerate Team Development
  </div>

  <div class="grid grid-cols-2 gap-8">
    <!-- Left side: Benefits -->
    <div v-click class="space-y-6">
      <div class="bg-[#143055]/10 p-6 rounded-lg border border-[#143055]/20">
        <h3 class="font-bold text-lg mb-4 flex items-center gap-2">
          <i class="i-mdi-rocket-launch text-[#143055]" />
          Key Benefits
        </h3>
        <ul class="space-y-3">
          <li class="flex items-center gap-2">
            <i class="i-mdi-check text-green-500" />
            Share task results across teams
          </li>
          <li class="flex items-center gap-2">
            <i class="i-mdi-check text-green-500" />
            Eliminate redundant operations
          </li>
          <li class="flex items-center gap-2">
            <i class="i-mdi-check text-green-500" />
            Reduce CI/CD pipeline times
          </li>
        </ul>
      </div>
    </div>
    <!-- Right side: Visual Diagram -->
    <div v-click class="relative">
      <!-- Central Cloud -->
      <div class="cache-cloud absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
        <div class="p-4 bg-[#143055]/10 rounded-full">
          <img src="../images/nx.png" alt="Nx logo" class="w-16 h-16" />
        </div>
      </div>
      <!-- Connecting Lines -->
      <svg class="absolute inset-0 w-full h-full" xmlns="http://www.w3.org/2000/svg">
        <line x1="50%" y1="50%" x2="50%" y2="10%" stroke="#143055" stroke-width="2" />
        <line x1="50%" y1="50%" x2="90%" y2="50%" stroke="#143055" stroke-width="2" />
        <line x1="50%" y1="50%" x2="50%" y2="90%" stroke="#143055" stroke-width="2" />
        <line x1="50%" y1="50%" x2="10%" y2="50%" stroke="#143055" stroke-width="2" />
      </svg>
      <!-- Developer Machines -->
      <div class="developers-circle relative">
        <div class="dev-point dev-1">
          <i class="i-mdi-laptop text-2xl"></i>
        </div>
        <div class="dev-point dev-2">
          <i class="i-mdi-laptop text-2xl"></i>
        </div>
        <div class="dev-point dev-3">
          <i class="i-mdi-laptop text-2xl"></i>
        </div>
        <div class="dev-point dev-4">
          <i class="i-mdi-laptop text-2xl"></i>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
.cache-cloud {
  z-index: 10;
}

.developers-circle {
  @apply w-64 h-64 mx-auto relative;
}

.dev-point {
  @apply absolute flex items-center justify-center p-2 bg-[#143055]/10 rounded-full;
}

.dev-1 { @apply top-0 left-1/2 -translate-x-1/2; }
.dev-2 { @apply top-1/2 right-0 -translate-y-1/2; }
.dev-3 { @apply bottom-0 left-1/2 -translate-x-1/2; }
.dev-4 { @apply top-1/2 left-0 -translate-y-1/2; }

/* Simplified layout ensures static lines connect machines to Nx */
</style>
