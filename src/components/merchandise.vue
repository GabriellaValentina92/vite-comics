<script>
export default {
  data() {
    return {
      shopsLink: [
        {
          image: "buy-comics-digital-comics.png",
          title: "DIGITAL COMICS",
        },

        {
          image: "buy-comics-merchandise.png",
          title: "DC MERCHANDISE",
        },

        {
          image: "buy-comics-subscriptions.png",
          title: "SUBSCRIPTION",
        },

        {
          image: "buy-comics-shop-locator.png",
          title: "COMIC SHOP LOCATOR",
        },

        {
          image: "buy-dc-power-visa.svg",
          title: "DC POWER VISA",
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
  <ul>
    <li class="shopOnline">
      <ul class="links" v-for="shop in shopsLink" :key="shop.title">
        <li>
          <img :src="getImagePath(shop.image)" :alt="shop.title" />
        </li>
        <li>{{ shop.title }}</li>
      </ul>
    </li>
  </ul>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
ul {
  background-color: rgb(7, 127, 246);
}

.shopOnline {
  @include container-size;
  @include merch-display-flex;
  min-height: 100px;
  .links {
    display: flex;
    align-items: center;
    list-style: none;
  }
}
.links li img {
  width: 30px;
  margin-right: 0.8rem;
}
</style>
