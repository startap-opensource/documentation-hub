<template>
  <div class="row px-10 py-10 bg-base-content">
    <h1 class="text-3xl font-bold my-5 text-accent-content">Backend Tools</h1>

    <div class="grid grid-flow-row grid-cols-4 gap-7">
      <div v-for="(tool, index) in backendTools" :key="index" class="card bg-base-200">
        <div class="card-body justify-center pb-5">

          <div class="justify-center">
            <img :src="getToolImage(tool.logo)" :alt="tool.name"
                 class="min-h-16 max-h-20 mx-auto">
          </div>

          <div class="tool__information">
<!--            <h3 class="card-title text-center">{{ tool.name }}</h3>-->

          </div>
        </div>

        <div class="card-footer">
          <a class="btn btn-block btn-wide btn-ghost rounded-none" :href="tool.url" target="_blank">
            Visit documentation
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import {phpTools, pythonTools} from "@/data/backend";

export default {
  name: "BackendTools",

  data() {
    return {
      backendTools: [
        ...phpTools,
        ...pythonTools,
      ],
    };
  },

  methods: {
    getToolImage(tool) {
      return tool === '' ? '' : require(`../../assets/logos/${tool}`);
    },
  }
}
</script>

<style scoped>

</style>