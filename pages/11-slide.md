---
layout: default
---

# Auto-Rerun Flaky Tasks

<div class="mt-12">
  <div v-click class="text-xl mb-8">
    Identify and re-run flaky tasks to ensure build stability.
  </div>
  <div class="grid grid-cols-2 gap-8">
    <div v-click class="space-y-6">
      <div class="bg-orange-50 dark:bg-orange-900 p-6 rounded-lg">
        <h3 class="font-bold text-lg mb-4">
          <i class="i-mdi-refresh mr-2" />
          Automatic Recovery
        </h3>
        <ul class="list-disc ml-4 space-y-2">
          <li>Detects flaky tests</li>
          <li>Automatic retries</li>
          <li>Failure analysis</li>
        </ul>
      </div>
    </div>
    <div v-click class="flex items-center justify-center">
      <div class="relative">
        <div class="task-status failed">
          <i class="i-mdi-close-circle text-2xl" />
          Failed
        </div>
        <div class="task-status retrying">
          <i class="i-mdi-refresh text-2xl animate-spin" />
          Retrying
        </div>
        <div class="task-status success">
          <i class="i-mdi-check-circle text-2xl" />
          Success
        </div>
      </div>
    </div>
  </div>
</div>

<style>
.task-status {
  @apply p-4 rounded-lg flex items-center gap-2 mb-4 transition-all duration-300;
}
.failed {
  @apply bg-red-100 dark:bg-red-900 text-red-700 dark:text-red-100;
}
.retrying {
  @apply bg-yellow-100 dark:bg-yellow-900 text-yellow-700 dark:text-yellow-100;
}
.success {
  @apply bg-green-100 dark:bg-green-900 text-green-700 dark:text-green-100;
}
</style>
