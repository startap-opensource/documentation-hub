<template>
  <div class="navbar mb-2 shadow-lg bg-neutral text-neutral-content">
    <div class="flex-none hidden lg:flex">
      <button class="btn btn-square btn-ghost">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
             class="inline-block w-6 h-6 stroke-current">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
        </svg>
      </button>
    </div>
    <div class="flex-1 hidden px-2 mx-2 lg:flex">
    <span class="text-lg font-bold">
            Documentation Hub
          </span>
    </div>
    <div class="flex-1 lg:flex-none">
      <div class="form-control">
        <input type="text" placeholder="Search" class="input input-ghost">
      </div>
    </div>

    <div class="flex-none">
      <a class="btn btn-square btn-ghost"
         href="https://github.com/startap/documentation-hub"
         target="_blank"
         title="See on GitHub"
         aria-label="See on GitHub">
        <Icon
            icon="fa-brands:github"
            class="text-2xl"/>
      </a>
    </div>
  </div>
</template>

<script>
import {Icon} from '@iconify/vue'

export default {
  name: "Cabecalho",
  components: {Icon},
}
</script>

<style scoped>

</style>