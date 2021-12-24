<template>
  <BaseHeader />
  <Homepage />
</template>

<script>
import BaseHeader from "@/components/BaseHeader";
import Homepage from '@/components/Home';

export default {
  name: 'App',
  components: { BaseHeader, Homepage }
}
</script>