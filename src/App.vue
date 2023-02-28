<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import BottomSection from "./components/BottomSection.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Header,
    Content,
    BottomSection,
    Footer,
  },
};
</script>

<template>
  <div class="">
    <header><Header /></header>
    <main>
      <div class="content"><Content /></div>
      <div><BottomSection /></div>
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
  padding: 3rem 0;
}
</style>
