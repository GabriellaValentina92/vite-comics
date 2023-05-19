<script>
export default {
  props: {
    ImageUrl: String,
    title: String,
  },
};
</script>

<template>
  <div class="cardComics">
    <img :src="ImageUrl" alt="title" />
    <h2>{{ title }}</h2>
  </div>
</template>

<style lang="scss" scoped>
.cardComics {
  max-width: 15%;
  line-height: 0.3rem;
  padding: 1rem;

  img {
    width: 150px;
    height: 150px;
    padding: 0.9rem;
    object-fit: cover;
    object-position: top;
  }

  h2 {
    color: white;
    font-size: 0.6rem;
    text-transform: uppercase;
    line-height: 0.6rem;
    margin-left: 1rem;
  }
}
</style>
