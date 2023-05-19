<script>
import navBar from "./navBar.vue";
export default {
  components: {
    navBar,
  },

  data() {
    return {
      logoImg: "dc-logo.png",
    };
  },

  methods: {
    getImagePath(img) {
      return new URL(`../assets/img/${img}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <ul class="navbar">
    <li class="logo">
      <img :src="getImagePath(logoImg)" alt="" />
    </li>
    <navBar />
  </ul>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
$bg-color: white;
.navbar {
  @include container-size;
  @include display-flex;

  .logo {
    list-style: none;
  }
  .logo img {
    width: 60px;
  }
}
</style>
