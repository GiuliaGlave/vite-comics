<script>
export default {
  data() {
    return {
      cards: [
        {
          img: "buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          img: "img2",
          text: "DC MERCHANDISE",
        },
        {
          img: "img3",
          text: "SUBSCRIPTION",
        },
        {
          img: "img4",
          text: "COMIC SHOP LOCATOR",
        },
        {
          img: "img5",
          text: "DC POWER VISA",
        },
      ],
    };
  },

  methods: {
    imgPath: function (img) {
      return new URL(`../assets/${img}`, import.meta.url).href;
    },
  },
};
</script>
<template>
  <div class="bottom-section">
    <ul v-for="card in cards">
      <li>
        <a href="#"
          ><div>
            <img
              :src="imgPath(img)"
              alt=""
            />
            {{ card.img }}
          </div>
          <div>{{ card.text }}</div></a
        >
      </li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;

.bottom-section,
a {
  @include align_list();
  @include bottom_section();
  justify-content: space-between;
  gap: 2rem;
}
</style>
