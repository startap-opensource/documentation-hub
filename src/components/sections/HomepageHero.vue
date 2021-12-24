<template>
  <div class="hero min-h-screen bg-base-200">
    <div class="flex-col hero-content lg:flex-row-reverse">
      <img :src="heroSvg" class="max-w-lg">
      <div>
        <h1 class="mb-5 text-5xl font-bold">
          A single place to find your documentation.
        </h1>
        <p class="mb-5">
          Find and search any documentation used on your project.
          <br>
          <i>(Or submit a pull request to update this amazing tool that we built together!)</i>
        </p>
        <button class="btn btn-primary">Search a tool</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HomepageHero',
  props: {
    heroSvg: {}
  }
}
</script>
