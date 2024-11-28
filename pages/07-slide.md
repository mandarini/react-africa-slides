---
layout: default
---

# Run Only Affected Tasks

<div class="flex mt-12">
  <div class="flex-1">
    <div v-click class="text-xl mb-8">
      Optimize builds by running only tasks affected by a PR.
    </div>
    <div v-click class="bg-blue-50 dark:bg-blue-900 p-6 rounded-lg">
      <h3 class="font-bold text-lg mb-4">
        <i class="i-mdi-graph mr-2" />
        Smart Task Execution
      </h3>
      <ul class="list-disc ml-4 space-y-2">
        <li>Analyzes dependency graph</li>
        <li>Identifies affected projects</li>
        <li>Skips unnecessary builds</li>
      </ul>
    </div>
  </div>

  <div v-click class="flex-1 ml-8">
    <div class="border dark:border-gray-700 rounded-lg p-4">
      <div class="text-center mb-4 font-bold">Dependency Graph Example</div>
      <div class="w-full h-64 bg-gray-100 dark:bg-gray-800 rounded flex items-center justify-center">
      <img 
      src="../images/dependency-graph.png" 
      alt="Dependency Graph Example" 
      />
      </div>
      <div class="text-sm text-center mt-4 text-gray-500">
        Pink nodes indicate affected projects
      </div>
    </div>
  </div>
</div>

<div class="absolute bottom-4 left-0 right-0 text-gray-400 text-sm text-center">
  @psybercity - @NxDevTools - 🦋 @psyber.city - 🦋 @nx.dev - Katerina Skroumpelou - AngularDay2024
</div>
