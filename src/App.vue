<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<template>
  <div class="container">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<style>
ul {
  list-style-type: none;
}

a {
  text-decoration: none;
}
</style>
