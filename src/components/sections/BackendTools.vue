<template>
  <div class="row px-10 py-10 bg-base-content">
    <h1 class="text-3xl font-bold my-5 text-accent-content">Backend Tools</h1>

    <div class="grid grid-flow-row grid-cols-4 gap-7">
      <div v-for="(tool, index) in backendTools.php" :key="index"
           class="card bg-base-200">
        <figure class="justify-center pt-10 pb-5 px-10">
          <img :src="getToolImage(tool.logo)" :alt="tool.name" class="max-h-20">
        </figure>
        <div class="card-body justify-between">
          <h3 class="card-title">{{ tool.name }}</h3>

          <div class="card-actions">
            <a class="btn btn-secondary btn-outline btn-sm text-xs" :href="tool.url" target="_blank">
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
  },

  methods: {
    getToolImage(tool) {
      return tool === '' ? '' : require(`../../assets/logos/${tool}`);
    }
  }
}
</script>

<style scoped>

</style>