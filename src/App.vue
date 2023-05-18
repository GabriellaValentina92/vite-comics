<script>
import Header from "./components/Header.vue";
import mainContent from "./components/mainContent.vue";
import merchandise from "./components/merchandise.vue";
import footer from "./components/footer.vue";

export default {
  components: {
    Header,
    mainContent,
    merchandise,
    footer,
  },
};
</script>

<template>
  <Header></Header>
  <mainContent></mainContent>
  <merchandise></merchandise>
  <footer></footer>
</template>

<style lang="scss">
@use "../src/style/general.scss" as *;
</style>
