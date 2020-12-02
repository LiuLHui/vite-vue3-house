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
    const width = document.documentElement.clientWidth
    const asideVisible = ref(width <= 500 ? false : true)
    provide('asideVisible',asideVisible)  // set
  }
};
</script>
<style lang="scss" scoped>
  
</style>