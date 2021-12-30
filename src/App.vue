<template>
  <div>
    <BaseHeader />
    <Homepage />
    <base-footer />
  </div>
</template>

<script>
import BaseHeader from "@/components/BaseHeader";
import Homepage from '@/components/Home';
import BaseFooter from "@/components/BaseFooter";

export default {
  name: 'App',
  components: { BaseHeader, Homepage, BaseFooter },
}
</script>