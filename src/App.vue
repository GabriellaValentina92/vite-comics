<script>
import Header from "./components/Header.vue";
import mainContent from "./components/mainContent.vue";
import merchandise from "./components/merchandise.vue";
import footer from "./components/footer.vue";
import signup from "./components/signup.vue";

export default {
  components: {
    Header,
    mainContent,
    merchandise,
    footer,
    signup,
  },
};
</script>

<template>
  <Header></Header>
  <mainContent></mainContent>
  <merchandise></merchandise>
  <footer></footer>
  <signup></signup>
</template>

<style lang="scss">
@use "../src/style/general.scss" as *;
</style>
