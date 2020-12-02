<template>
  <div>
    <router-view />
  </div>
</template>

<script lang="ts">
import { provide, ref } from 'vue';
export default {
  name: "App",
  setup(){
    const asideVisible = ref(false)
    provide('xxx',asideVisible)  // set
  }
};
</script>
<style lang="scss" scoped>
  
</style>