<script></script>

<template>
  <header>
    <div class="logo">
      <img
        src="../assets/img/dc-logo.png"
        alt=""
      />
    </div>
    <div class="nav">
      <ul>
        <li><a href="#">CHARACTERS</a></li>
        <li><a href="#">COMICS</a></li>
        <li><a href="#">MOVIES</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">GAMES</a></li>
        <li><a href="#">COLLECTIBLES</a></li>
        <li><a href="#">VIDEOS</a></li>
        <li><a href="#">FANS</a></li>
        <li><a href="#">NEWS</a></li>
        <li><a href="#">SHOP</a></li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;

header {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: stretch;
}

.nav {
  @include align_list();

  a {
    @include dark_color_text();

    font-weight: bold;
    display: flex;
    align-items: center;
    height: 100%;
    &:hover {
      @include primary_color_text();
      @include nav_hover();
    }
  }
}
</style>
