<template>
  <div class="row px-10 py-10 bg-base-content">
    <h2 class="text-3xl font-bold my-10 text-accent-content">Backend Tools</h2>

    <div class="grid grid-flow-row grid-cols-4 gap-7">
      <div v-for="(tool, index) in backendTools['phpTools']" :key="index"
           class="card shadow-2xl lg:card-side bg-base-200">
        <div class="card-body justify-between">
          <h3 class="card-title">{{ tool.name }}</h3>
          <span class="badge badge-primary badge-outline">{{ tool.language }}</span>

          <div class="card-actions">
            <a class="btn btn-secondary btn-outline text-sm" :href="tool.url">
              Visit documentation

              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                   class="inline-block w-6 h-6 ml-2 stroke-current">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
              </svg>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { phpTools, pythonTools } from "@/data/backend";

export default {
  name: "BackendTools",

  data() {
    return {
      backendTools: {
        php: phpTools,
        python: pythonTools,
      }
    };
  }
}
</script>

<style scoped>

</style>