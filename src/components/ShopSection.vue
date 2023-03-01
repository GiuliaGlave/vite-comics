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
          img: "buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "SUBSCRIPTION",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ],
    };
  },

  methods: {
    getImagePath: function (img) {
      return new URL(`../assets/img/${img}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="shop-section">
    <ul v-for="card in cards">
      <li>
        <a href="#"
          ><div>
            <img
              :src="getImagePath(card.img)"
              alt=""
            />
          </div>
          <div>{{ card.text }}</div></a
        >
      </li>
    </ul>
  </div>
</template>
<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;

.shop-section,
a {
  @include align_list();
  @include shop_section();
  justify-content: space-between;
  gap: 2rem;
}
</style>
