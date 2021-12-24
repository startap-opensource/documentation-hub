<template>
  <homepage-hero />
  <backend-tools />
  <frontend-tools />
</template>

<script>
import HomepageHero from "@/components/sections/HomepageHero"
import BackendTools from '@/components/sections/BackendTools'
import FrontendTools from "@/components/sections/FrontendTools"

export default {
  name: "Homepage",
  components: {HomepageHero, BackendTools, FrontendTools},
}
</script>