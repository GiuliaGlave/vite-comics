<script></script>

<template>
  <div class="container">
    <div>
      <button>SIGN-UP NOW!</button>
    </div>

    <div class="icons">
      <div>FOLLOW US</div>
      <ul>
        <li>
          <a href="#"><i class="fa-brands fa-twitter"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-facebook"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-instagram"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-pinterest"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-youtube"></i></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;
.container,
.icons {
  @include align_row();
}
</style>
