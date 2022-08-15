<template>
  <nav class="category">
    <p class="title">{{ title }}</p>
    <NavItem
      v-for="item in items"
      :key="item.id"
      :icon="item.icon"
      :title="item.title"
      :link="item.link"
    />
  </nav>
</template>

<script>
import NavItem from "./NavItem.vue";

export default {
  components: { NavItem },
  props: ["title", "items"],
};
</script>

<style scoped>
.category {
  display: flex;
  flex-direction: column;
  width: 100%;
  padding: 0px 20px 20px 20px;
}
.title {
}
</style>
