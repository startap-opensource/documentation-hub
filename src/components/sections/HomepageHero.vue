<template>
  <div class="hero min-h-screen bg-base-200">
    <div class="flex-col-reverse hero-content lg:flex-row">
      <div class="max-w-2xl">
        <h1 class="animate__animated animate__fadeIn animate__faster animate__delay-2s mb-5 text-5xl font-bold">
          A single place to find your documentation.
        </h1>

        <p class="mb-5 animate__animated animate__fadeIn animate__delay-2s animate__faster">
          Find and search any documentation used on your project.
          <br>
          <i>(Or submit a pull request to update this amazing tool that we built together!)</i>
        </p>
        <div class="animate__animated animate__fadeInUp animate__delay-2s animate__fast">
          <button class="btn btn-primary">Search a tool</button>
        </div>
      </div>

      <HeroImage/>
    </div>
  </div>
</template>
<script>
import HeroImage from "@/components/sections/HeroImage";

export default {
  name: 'HomepageHero',
  components: {HeroImage},
}
</script>