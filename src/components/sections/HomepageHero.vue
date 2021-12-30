<template>
  <div class="hero min-h-screen">
    <div class="hero-content flex-col pt-24 md:pt-0 md:flex-row pt-2">
      <div class="max-w-2xl text-center md:text-left">
        <h1 class="animate__animated animate__slideInUp animate__faster mb-5 text-5xl font-bold">
          A Developer's Documentation Hub.
        </h1>

        <p class="mb-5 animate__animated animate__slideInUp animate__faster">
          Find the documentation that you need to your project. It's all in one place.
        </p>
        <div class="animate__animated animate__slideInUp animate__fast">
          <a
            class="btn btn-primary"
            href="#container-tools"
          >
            See all tools
          </a>
        </div>
      </div>
      <HeroImage />
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
