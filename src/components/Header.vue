<script>
export default {
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
        },
        {
          text: "COMICS",
        },
        {
          text: "MOVIES",
        },
        {
          text: "TV",
        },
        {
          text: "GAMES",
        },
        {
          text: "COLLECTIBLES",
        },
        {
          text: "VIDEOS",
        },
        {
          text: "FANS",
        },
        {
          text: "NEWS",
        },
        {
          text: "SHOP",
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="logo">
      <img
        src="../assets/img/dc-logo.png"
        alt=""
      />
    </div>
    <div class="nav">
      <ul v-for="link in links">
        <li>
          <a href="#"> {{ link.text }} </a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;
@use "../assets/styles/partials/variables.scss" as *;

header {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: stretch;
}

.nav {
  @include align_list();

  a {
    color: $dark_color;
    margin: 0 1rem;
    font-weight: bold;
    display: flex;
    align-items: center;
    height: 100%;
    &:hover {
      color: $primary_color;
      @include nav_hover();
    }
  }
}
</style>
