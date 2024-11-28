---
layout: default
---

<div class="title-container">
  <h1>Why React Developers Love Nx</h1>
</div>

<div class="mt-12 grid grid-cols-3 gap-8 px-4">
  <!-- Code Generators Box -->
  <div v-click class="feature-box group">
    <div class="icon-wrapper" style="--accent-color: #61DAFB;">
      <i class="i-mdi-code-braces text-4xl"></i>
    </div>
    <h3 class="text-xl font-bold mt-4 mb-2">Code Generators</h3>
    <div class="terminal-window">
      <span class="typing-text">> nx g @nx/react:app</span>
      <span class="cursor">_</span>
    </div>
  </div>

  <!-- Automatic Migrations Box -->
  <div v-click class="feature-box group">
    <div class="icon-wrapper" style="--accent-color: #4CAF50;">
      <i class="i-mdi-update text-4xl rotating"></i>
    </div>
    <h3 class="text-xl font-bold mt-4 mb-2">Automatic Migrations</h3>
    <div class="progress-bar">
      <div class="progress-fill"></div>
    </div>
  </div>

  <!-- Workspace Insights Box -->
  <div v-click class="feature-box group">
    <div class="icon-wrapper" style="--accent-color: #FF4081;">
      <i class="i-mdi-chart-line text-4xl sparkle"></i>
    </div>
    <h3 class="text-xl font-bold mt-4 mb-2">Workspace Insights</h3>
    <div class="graph-animation">
      <svg viewBox="0 0 100 40" class="line-chart">
        <path d="M0,35 L20,25 L40,30 L60,15 L80,20 L100,5" class="chart-line"></path>
      </svg>
    </div>
  </div>
</div>

<style>
.title-container {
  text-align: center;
  margin-top: 2rem;
}

.feature-box {
  @apply bg-gray-800/50 backdrop-blur-sm p-6 rounded-xl border border-gray-700/50 
         transition-all duration-300 hover:transform hover:-translate-y-1 hover:shadow-xl;
}

.icon-wrapper {
  @apply w-16 h-16 rounded-full flex items-center justify-center mb-4 mx-auto
         transition-transform duration-300 bg-opacity-20;
  background-color: var(--accent-color);
}

.group:hover .icon-wrapper {
  @apply transform scale-110;
}

/* Terminal Animation */
.terminal-window {
  @apply bg-black/50 p-3 rounded-lg mt-4 font-mono text-sm;
}

.cursor {
  animation: blink 1s infinite;
}

@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}

/* Progress Bar Animation */
.progress-bar {
  @apply bg-gray-700 rounded-full h-2 mt-4 overflow-hidden;
}

.progress-fill {
  @apply h-full bg-[#4CAF50] rounded-full;
  animation: fill 3s infinite;
  width: 0%;
}

@keyframes fill {
  0% { width: 0%; }
  100% { width: 100%; }
}

/* Rotating Animation */
.rotating {
  animation: rotate 4s linear infinite;
}

@keyframes rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

/* Chart Animation */
.line-chart {
  @apply w-full h-12 mt-4;
}

.chart-line {
  fill: none;
  stroke: var(--accent-color);
  stroke-width: 2;
  stroke-dasharray: 200;
  stroke-dashoffset: 200;
  animation: draw 3s ease-out forwards infinite;
}

@keyframes draw {
  to {
    stroke-dashoffset: 0;
  }
}

/* Sparkle Animation */
.sparkle {
  animation: sparkle 2s ease-in-out infinite;
}

@keyframes sparkle {
  0%, 100% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.2); opacity: 0.8; }
}
</style>

<!--
Nx is designed with developer experience in mind, automating repetitive tasks and simplifying maintenance.
From generating boilerplate code to running guided migrations, Nx helps you focus on what you do best: building amazing apps.
-->