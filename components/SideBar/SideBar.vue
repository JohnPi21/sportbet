<template>
  <div class="sidebar">
    <NavCategory
      v-for="category in categories"
      :key="category.id"
      :title="category.title"
      :items="category.items"
      :link="category.link"
    />
  </div>
</template>
<script>
import NavCategory from "./NavCategory.vue";

export default {
  components: { NavCategory },
  data: () => ({
    categories: [
      {
        id: 1,
        title: "Navigation",
        items: [
          { id: 1, icon: "casa", title: "Home", link: "#" },
          { id: 2, icon: "live", title: "Live", link: "#" },
          { id: 3, icon: "star", title: "Favorites", link: "#" },
          { id: 4, icon: "ball", title: "Fotball", link: "#" },
        ],
      },
      {
        id: 1,
        title: "Sport",
        link: "#",
        items: [
          { id: 1, icon: "football", title: "Football", link: "#" },
          { id: 2, icon: "tennis", title: "Tennis", link: "#" },
          { id: 3, icon: "volleyball", title: "Volleyball", link: "#" },
          { id: 4, icon: "ice hockey", title: "Ice Hockey", link: "#" },
        ],
      },
    ],
  }),
};
</script>

<style scoped>
.sidebar {
  min-width: var(--sidebar-width);
  width: var(--sidebar-width);
  height: 100%;
  position: fixed;
  left: 0;
  background: var(--sidebar-background);
  color: var(--sidebar-text-color);
}
</style>
