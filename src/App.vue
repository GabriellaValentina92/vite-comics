<script>
import Header from "./components/Header.vue";
import mainContent from "./components/mainContent.vue";
import merchandise from "./components/merchandise.vue";
import secFooter from "./components/secFooter.vue";
import signup from "./components/signup.vue";
import jumbotron from "./components/jumbotron.vue";

export default {
  components: {
    Header,
    mainContent,
    merchandise,
    secFooter,
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
  <secFooter></secFooter>
  <signup></signup>
</template>

<style lang="scss">
@use "../src/style/general.scss" as *;
</style>
