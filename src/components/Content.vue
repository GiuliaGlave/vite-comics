<script>
export default {
  data() {
    return {
      jumbotron: {
        img: "jumbotron.jpg",
      },
      comics: [
        {
          cover: "buy-comics-shop-locator.png",
          title: "titolo",
        },
        {
          cover: "copertina",
          title: "titolo",
        },
        {
          cover: "copertina",
          title: "titolo",
        },
        {
          cover: "copertina",
          title: "titolo",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="jumbotron">
    <img
      :src="jumbotron.img"
      alt=""
      src="../assets/img/buy-comics-digital-comics.png"
    />
  </div>
  <div class="comics">
    <ul v-for="comic in comics">
      <li>
        <a href="#"
          ><div class="bg-danger">
            <img
              :src="comic.cover"
              alt=""
            />
          </div>
          <div>{{ comic.title }}</div>
        </a>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;
ul {
  @include align_div();
}
</style>
