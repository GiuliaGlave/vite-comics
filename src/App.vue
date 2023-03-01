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
  <div class="">
    <header><Header /></header>
    <main>
      <div class="content"><Content /></div>
      <div><ShopSection /></div>
    </main>
    <footer><Footer /></footer>
  </div>
</template>

<style lang="scss">
@use "./assets/styles/generals.scss";
@use "./assets/styles/partials/mixins.scss" as *;

header {
  @include align_list();
}

main {
  @include dark_color_bg();
  padding: 0;
  margin: 0;
}
.content {
  @include light_color_text();
}
</style>
