<script></script>

<template>
  <!-- FOOTER TOP -->
  <div class="container-fluid">
    <div class="footer-content-left col-4 d-flex py-4">
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
    <div class="footer-content-right col-6">
      <!-- <img
        src="../assets/img/dc-logo-bg.png"
        alt=""
      /> -->
    </div>
  </div>

  <div class="container-bottom">
    <div>
      <button>SIGN-UP NOW!</button>
    </div>

    <div class="icons">
      <div class="px-4 text-primary fw-bold">FOLLOW US</div>
      <ul>
        <li>
          <a href="#"
            ><img
              src="../assets/img/footer-facebook.png"
              alt=""
          /></a>
        </li>

        <li>
          <a href="#"
            ><img
              src="../assets/img/footer-twitter.png"
              alt=""
          /></a>
        </li>

        <li>
          <a href="#"
            ><img
              src="../assets/img/footer-youtube.png"
              alt=""
          /></a>
        </li>

        <li>
          <a href="#"
            ><img
              src="../assets/img/footer-pinterest.png"
              alt=""
          /></a>
        </li>

        <li>
          <a href="#"
            ><img
              src="../assets/img/footer-periscope.png"
              alt=""
          /></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;

.container-bottom,
.icons {
  @include align_list();
  background-color: #303030;
  padding: 1rem 0;
}
.container-fluid {
  @include footer_style();
  @include align_div();
  height: fit-content;
}

.footer-content-right {
  background-image: url(../assets/img/dc-logo-bg.png);
  height: 100%;
}
button {
  @include button_hover();
}
</style>
