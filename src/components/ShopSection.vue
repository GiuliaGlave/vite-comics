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
  <div class="shop-section content">
    <ul class="content">
      <li v-for="card in cards">
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
  @include shop_section();
}

ul {
  @include flex-center();
  gap: 2rem;

  li {
    a {
      @include flex-center();
      gap: 2rem;

      div {
        img {
          min-width: 5rem;
          aspect-ratio: 1;
          object-fit: contain;
        }
      }
    }
  }
}

.content {
  @include margin_app();
}
</style>
