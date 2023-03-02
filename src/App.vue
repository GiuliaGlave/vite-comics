<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import ShopSection from "./components/ShopSection.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Header,
    Content,
    ShopSection,
    Footer,
  },
};
</script>

<template>
  <div>
    <header class="content"><Header /></header>
    <main>
      <div><Content /></div>
      <div><ShopSection /></div>
    </main>
    <footer><Footer /></footer>
  </div>
</template>

<style lang="scss">
@use "./assets/styles/generals.scss";
@use "./assets/styles/partials/mixins.scss" as *;
@use "./assets/styles/partials/variables.scss" as *;

.app-container {
}
header {
  @include align_list();
}

main {
  background-color: $dark_color;
  padding: 0;
  margin: 0;
}
</style>
