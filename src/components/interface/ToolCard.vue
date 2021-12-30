<template>
  <div class="card bg-base-200">
    <div class="card-body justify-center pb-5">
      <div class="justify-center">
        <img
          :src="getToolImage(currentTool.logo)"
          :alt="currentTool.name"
          class="min-h-16 max-h-20 mx-auto"
        >
      </div>

      <div class="tool__information" />
    </div>

    <div class="card-footer">
      <a
        class="btn btn-block btn-wide btn-outline btn-info border-0 rounded-none"
        :href="currentTool.url"
        target="_blank"
      >
        <i class="mr-2 h-100">
          <svg
            aria-hidden="true"
            focusable="false"
            height="1rem"
            data-prefix="fas"
            data-icon="external-link-alt"
            class="svg-inline--fa fa-external-link-alt fa-w-16"
            role="img"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
          ><path
            fill="currentColor"
            d="M432,320H400a16,16,0,0,0-16,16V448H64V128H208a16,16,0,0,0,16-16V80a16,16,0,0,0-16-16H48A48,48,0,0,0,0,112V464a48,48,0,0,0,48,48H400a48,48,0,0,0,48-48V336A16,16,0,0,0,432,320ZM488,0h-128c-21.37,0-32.05,25.91-17,41l35.73,35.73L135,320.37a24,24,0,0,0,0,34L157.67,377a24,24,0,0,0,34,0L435.28,133.32,471,169c15,15,41,4.5,41-17V24A24,24,0,0,0,488,0Z"
          /></svg>
        </i>
        <span>{{ currentTool.name }}</span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "ToolCard",

  props: {
    currentTool: {
      type: Object,
      required: true,
    }
  },

  methods: {
    getToolImage(logoImage) {
      if (logoImage)
        return require(`/src/assets/logos/${logoImage}`)

      return ''
    },
  }
}
</script>

<style scoped>

</style>