<template>
  <div class="app">
    <NavBar class="navbar" />
    <div class="main-container">
      <SideBar class="sidebar" />
      <Nuxt />
    </div>
  </div>
</template>

<script>
import SideBar from "~/components/SideBar/SideBar.vue";
import NavBar from "~/components/NavBar.vue";
export default {
  components: { SideBar, NavBar },
};
</script>
<style scoped>
.app {
  width: 100vw;
}
.main-container {
  width: 100%;
  height: calc(100vh - var(--navbar-height));
  display: flex;
}
</style>
