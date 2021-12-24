<template>
  <homepage-hero />

  <div class="my-2">
    <backend-tools></backend-tools>
  </div>
</template>

<script>
import BackendTools from '@/components/sections/BackendTools'
import HomepageHero from "@/components/sections/HomepageHero";

export default {
  name: "Homepage",
  components: {HomepageHero, BackendTools},
}
</script>