<script>
import Header from "./components/Header.vue";
import mainContent from "./components/mainContent.vue";
import merchandise from "./components/merchandise.vue";
import footer from "./components/footer.vue";
import signup from "./components/signup.vue";
import jumbotron from "./components/jumbotron.vue";

export default {
  components: {
    Header,
    mainContent,
    merchandise,
    footer,
    signup,
    jumbotron,
  },
};
</script>

<template>
  <Header></Header>
  <jumbotron></jumbotron>
  <mainContent></mainContent>
  <merchandise></merchandise>
  <footer></footer>
  <signup></signup>
</template>

<style lang="scss">
@use "../src/style/general.scss" as *;
</style>
