<template>
  <header>This is top navbar</header>
</template>

<script>
export default {};
</script>

<style scoped>
.navbar {
  background: var(--navbar-background);
  color: var(--navbar-text-color);
  height: var(--navbar-height);
  width: 100%;
  position: sticky;
  position: -webkit-sticky;
  top: 0; /* required */
}
</style>
