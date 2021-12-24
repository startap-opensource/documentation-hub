<template>
  <div class="row px-10 py-10 row px-10 py-10 bg-gradient-to-br from-gray-600 to-gray-800">
    <h1 class="text-3xl font-bold my-5 text-accent-content">Frontend Tools</h1>

    <div class="grid grid-flow-row grid-cols-4 gap-7">
      <tool-card v-for="(tool, index) in frontendTools"
                 :key="index"
                 :current-tool="tool">
      </tool-card>
    </div>
  </div>
</template>

<script>
import {FrontendTools} from "@/data/frontend";
import ToolCard from "@/components/interface/ToolCard";

export default {
  name: "FrontendTools",
  components: {
    ToolCard
  },

  data() {
    return {
      frontendTools: FrontendTools,
    };
  },
}
</script>

<style scoped>

</style>