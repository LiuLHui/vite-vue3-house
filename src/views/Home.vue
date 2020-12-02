<template>
  <div>
    <Topnav></Topnav>
    <div class="banner">
      <h1>demoUI</h1>
      <h1>XXXXXXXXXXXXXXX</h1>
      <p class="actions">
        <a>github</a>
        <router-link to='/doc'>开始</router-link>
      </p>
    </div>
  </div>
</template>
<style lang="scss" scoped></style>
<script>
import Topnav from "../components/Topnav.vue";
export default {
  components: {
    Topnav,
  },
};
</script>

<style lang="scss" scoped>
.banner {
  padding: 100px 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background: lightgreen;
  > .actions {
    padding: 8px 0;
    a {
      margin: 0 8px;
      background: #fff;
      display: inline-block;
      $h: 28px;
      height: $h;
      line-height: $h;
      border-radius: $h/2;
      padding: 0 8px;
    }
  }
}
</style>
