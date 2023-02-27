<script></script>

<template>
  <!-- FOOTER TOP -->
  <div class="container-top">
    <div class="footer-content col-4 d-flex py-4">
      <!-- dc comics -->
      <div class="footer-list px-3">
        <div class="title">DC COMICS</div>
        <ul>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>Tv</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
      </div>
      <!-- shop -->
      <div class="footer-list px-3">
        <div class="title">SHOP</div>
        <ul>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div>
      <!-- dc -->
      <div class="footer-list px-3">
        <div class="title">DC</div>
        <ul>
          <li>Terms Of Use</li>
          <li>Privacy policy (New)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
      </div>
      <!-- sites -->
      <div class="footer-list px-3">
        <div class="title">SITE</div>
        <ul>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="container-bottom">
    <div>
      <button>SIGN-UP NOW!</button>
    </div>

    <div class="icons">
      <div class="px-4">FOLLOW US</div>
      <ul>
        <li>
          <a href="#"><i class="fa-brands fa-facebook"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-twitter"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-youtube"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-brands fa-pinterest"></i></a>
        </li>

        <li>
          <a href="#"><i class="fa-solid fa-location-dot"></i></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;
.container-bottom,
.icons {
  @include align_row();
}
</style>
