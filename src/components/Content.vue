<script>
export default {
  data() {
    return {
      jumbotron: {
        img: "jumbotron.jpg",
      },
    };
  },

  methods: {
    getImagePath: function (img) {
      return new URL(`../assets/img/${img}`, import.meta.url).href;
    },
  },
  props: {
    comics: Array,
  },
};
</script>

<template>
  <div class="jumbotron">
    <img
      :src="getImagePath(jumbotron.img)"
      alt=""
      class="jumbotron"
    />
  </div>
  <div class="position-relative">
    <span class="label fs-1">CURRENT SERIES</span>
  </div>

  <section class="pt-5">
    <ul class="my-5">
      <li
        v-for="comic in comics"
        :key="comic.series"
        class="mb-4"
      >
        <a href="#">
          <div class="cover">
            <img
              :src="comic.thumb"
              alt=""
            />
          </div>
          <div class="series">{{ comic.series }}</div>
        </a>
      </li>
    </ul>
    <div class="d-flex justify-content-center mb-4">
      <button>LOAD MORE</button>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;
@use "../assets/styles/partials/variables.scss" as *;
.jumbotron {
  object-fit: cover;
  object-position: top;
  width: 100%;
  height: 40vh;
}
section {
  max-width: 80%;
  margin: 0 auto;
}

span {
  position: absolute;
  bottom: -3rem;
  left: 10rem;
}

.label,
button {
  @include label();
}

ul {
  display: flex;
  flex-wrap: wrap;

  li {
    width: calc((100% / 6));

    a {
      color: $light_color;
      flex-direction: column;
      display: flex;
      width: 100%;
      gap: 1rem;
      padding: 1rem;
      .cover {
        img {
          object-fit: cover;
          object-position: top;
          width: 100%;
          aspect-ratio: 1;
        }
      }
      .series {
        font-size: 1rem;
      }
    }
  }
}
</style>
