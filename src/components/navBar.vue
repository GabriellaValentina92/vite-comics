<script>
export default {
  data() {
    return {
      arrMenu: [
        {
          name: "CHARACTER",
          src: "#",
        },

        {
          name: "TV",
          src: "#",
        },

        {
          name: "COMICS",
          src: "#",
        },

        {
          name: "GAMES",
          src: "#",
        },

        {
          name: "COLLECTIBLES",
          src: "#",
        },

        {
          name: "VIDEOS",
          src: "#",
        },

        {
          name: "FANS",
          src: "#",
        },

        {
          name: "NEWS",
          src: "#",
        },

        {
          name: "SHOPS",
          src: "#",
        },
      ],
    };
  },
};
</script>

<template>
  <ul class="nav-menu">
    <li v-for="element in arrMenu" :key="element.name">
      <a :href="element.src"> {{ element.name }}</a>
    </li>
  </ul>
</template>

<style lang="scss" scoped>
.nav-menu {
  display: flex;

  li {
    font-weight: 500;
    list-style: none;
    padding: 0.5rem;
  }

  li a {
    text-decoration: none;
    color: black;
  }
}
</style>
