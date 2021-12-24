<template>
  <div class="row px-10 py-10 row px-10 py-10 bg-gradient-to-br from-indigo-800 to-indigo-900">
    <h1 class="text-3xl font-bold my-5 text-accent-content">Backend Tools</h1>

    <div class="grid grid-flow-row grid-cols-4 gap-7">
      <tool-card v-for="(tool, index) in backendTools"
                 :key="index"
                 :current-tool="tool">
      </tool-card>
    </div>
  </div>
</template>

<script>
import {phpTools, pythonTools} from "@/data/backend";
import ToolCard from "@/components/interface/ToolCard";

export default {
  name: "BackendTools",
  components: {
    ToolCard
  },

  data() {
    return {
      backendTools: [
        ...phpTools,
        ...pythonTools,
      ],
    };
  },
}
</script>

<style scoped>

</style>