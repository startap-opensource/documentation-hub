<template>
  <div class="card bg-base-200">
    <div class="card-body justify-center pb-5">

      <div class="justify-center">
        <img :src="getToolImage(currentTool.logo)" :alt="currentTool.name"
             class="min-h-16 max-h-20 mx-auto">
      </div>

      <div class="tool__information">
      </div>
    </div>

    <div class="card-footer">
      <a class="btn btn-block btn-wide btn-outline btn-info border-0 rounded-none" :href="currentTool.url" target="_blank">
        Visit documentation
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "ToolCard.vue",

  props: {
    currentTool: {
      type: Object,
      required: true,
    }
  },

  methods: {
    getToolImage(logoImage) {
      return require(`/src/assets/logos/${logoImage}`);
    },
  }
}
</script>

<style scoped>

</style>