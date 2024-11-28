---
layout: default
---

# Distributed Task Execution (Nx Agents)

<div class="mt-8">
  <div v-click class="text-xl text-center mb-8">
    Distribute tasks across machines for faster builds
  </div>

  <div class="relative flex justify-center items-center h-[400px]">
    <!-- Central Nx Node -->
    <div v-click class="central-node">
      <div class="p-4 bg-[#143055]/10 rounded-full">
        <img src="../images/nx.png" alt="Nx logo" class="w-16 h-16" />
      </div>
    </div>
    <!-- Distributed Agents -->
    <div class="agents-circle">
      <div v-for="i in 3" :key="i" :class="`agent agent-${i}`">
        <div class="agent-icon">
          <i class="i-mdi-server text-2xl"></i>
        </div>
        <!-- Task Box -->
        <div class="task-box">
          <div class="task-progress"></div>
        </div>
        <!-- Checkmark -->
        <div class="checkmark">
          <i class="i-mdi-check text-green-500"></i>
        </div>
      </div>
    </div>
    <!-- Connection Lines -->
    <svg class="connection-lines" viewBox="0 0 200 200">
      <line v-for="i in 3" :key="i" :class="`connection line-${i}`" x1="100" y1="100" :x2="100 + 80 * Math.cos(i * 2 * Math.PI / 3)" :y2="100 + 80 * Math.sin(i * 2 * Math.PI / 3)" />
    </svg>
  </div>
</div>

<style>
.central-node {
  @apply absolute z-10;
  animation: pulse 2s infinite ease-in-out;
}

.agents-circle {
  @apply absolute w-[300px] h-[300px];
}

.agent {
  @apply absolute p-4 bg-[#143055]/10 rounded-lg;
  opacity: 0;
  animation: fadeIn 0.5s forwards;
}

.agent-1 { 
  @apply top-0 left-1/2 -translate-x-1/2;
  animation-delay: 0.5s;
}
.agent-2 { 
  @apply bottom-1/4 -right-8;
  animation-delay: 1s;
}
.agent-3 { 
  @apply bottom-1/4 -left-8;
  animation-delay: 1.5s;
}

.agent-icon {
  @apply bg-white/90 p-3 rounded-lg shadow-lg mb-2;
}

.task-box {
  @apply w-full h-2 bg-gray-200 rounded-full overflow-hidden mt-2;
  opacity: 0;
  animation: fadeIn 0.3s forwards 2s;
}

.task-progress {
  @apply h-full bg-green-500 w-0;
  animation: progress 1.5s ease-out forwards 2.5s;
}

.checkmark {
  @apply absolute top-2 right-2;
  opacity: 0;
  transform: scale(0);
  animation: popIn 0.3s ease-out forwards 4s;
}

.connection-lines {
  @apply absolute w-full h-full;
}

.connection {
  @apply stroke-[#143055] stroke-2;
  stroke-dasharray: 10;
  animation: dash 1s linear infinite;
  opacity: 0.3;
}

@keyframes pulse {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.05); }
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes progress {
  from { width: 0; }
  to { width: 100%; }
}

@keyframes popIn {
  from { opacity: 0; transform: scale(0); }
  to { opacity: 1; transform: scale(1); }
}

@keyframes dash {
  to { stroke-dashoffset: -20; }
}
</style>
