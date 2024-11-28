---
layout: default
---

# CIPE Affected Project Graph

<div class="mt-8">
  <div v-click class="text-xl mb-8">
    Helps visualize project relationships and troubleshoot CI issues.
  </div>

  <div class="grid grid-cols-2 gap-8">
    <div v-click class="bg-purple-50 dark:bg-purple-900 p-6 rounded-lg">
      <h3 class="font-bold text-lg mb-4">
        <i class="i-mdi-graph-outline mr-2" />
        Project Dependencies
      </h3>
      <ul class="list-disc ml-4 space-y-2">
        <li>Visualize project relationships</li>
        <li>Identify affected projects</li>
        <li>Troubleshoot CI issues</li>
      </ul>
    </div>
  <div v-click class="flex-1 ml-8">
    <div class="border dark:border-gray-700 rounded-lg p-4">
      <div class="text-center mb-4 font-bold">Affected Project Graph</div>
      <div class="w-full h-64 bg-gray-100 dark:bg-gray-800 rounded flex items-center justify-center">
        <img 
        src="../images/affected-project-graph.png" 
        alt="Affected Project Graph" 
        />
      </div>
      <div class="text-sm text-center mt-4 text-gray-500">
        Blue nodes indicate affected projects
      </div>
    </div>
  </div>
  </div>
</div>

