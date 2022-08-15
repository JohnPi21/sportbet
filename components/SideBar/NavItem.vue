<template>
  <NuxtLink :to="link" class="item">
    <img :src="icon" class="item-image" />
    <span>{{ title }}</span>
  </NuxtLink>
</template>

<script>
export default {
  props: ["icon", "title", "link"],
};
</script>

<style scoped>
.item {
  display: flex;
  align-items: center;
  text-decoration: none;
}
.item-image {
  border-radius: 50%;
  width: 28px;
  height: 28px;
  margin-right: 5px;
}
</style>
