<script>
export default {
  data() {
    return {
      socialLinks: [
        {
          icon: "footer-facebook.png",
        },

        {
          icon: "footer-periscope.png",
        },

        {
          icon: "footer-pinterest.png",
        },

        {
          icon: "footer-twitter.png",
        },

        {
          icon: "footer-youtube.png",
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
  <div class="bg-color">
    <div class="container">
      <div class="signUp"><a href="#">SIGN-UP NOW!</a></div>
      <div class="icons">
        <h2>FOLLOW US</h2>
        <img
          v-for="icons in socialLinks"
          :key="icons.icon"
          :src="getImagePath(icons.icon)"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
.bg-color {
  background-color: black;
  padding: 0.5rem;

  .container {
    @include container-size;
    @include display-flex;

    .signUp {
      border: 2px solid rgb(17, 138, 237);
      padding: 0.5rem 1rem;
    }

    .signUp a {
      text-decoration: none;
      color: white;
    }

    .icons {
      display: flex;
      align-items: center;
    }
    .icons h2 {
      color: rgb(17, 138, 237);
      font-size: 1rem;
      padding: 0.5rem;
    }

    .icons img {
      padding: 0.5rem;
    }
  }
}
</style>
