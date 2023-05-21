<script>
export default {
  data() {
    return {
      dcLogoBig: "dc-logo-bg.png",

      fooMenu: [
        {
          title: "",
        },
      ],
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
  <ul class="footer-bg">
    <li class="footer-menu">
      DC COMICS
      <ul>
        <li>characters</li>
        <li>comics</li>
        <li>movies</li>
        <li>tv</li>
        <li>games</li>
        <li>videos</li>
        <li>news</li>
      </ul>
    </li>

    <li>
      <img :src="getImagePath(dcLogoBig)" alt="" />
    </li>
  </ul>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
.footer-bg {
  height: 300px;
  @include container-size;
  @include display-flex;
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;

  .footer-menu {
    color: black;
  }
}
</style>
