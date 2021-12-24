<template>
  <homepage-hero :hero-svg="heroSvg"/>

  <div class="my-2">
    <backend-tools></backend-tools>
  </div>
</template>

<script>
import heroSvg from '@/assets/illustrations/programming.svg'

import BackendTools from '@/components/sections/BackendTools'
import HomepageHero from "@/components/sections/HomepageHero";

export default {
  name: "Homepage",
  components: {HomepageHero, BackendTools},
  setup() {
    return {
      heroSvg
    }
  },
}
</script>