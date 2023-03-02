<script></script>

<template>
  <footer>
    <!-- FOOTER TOP -->
    <div class="footer-top content">
      <div class="footer-content-left">
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
          <!-- shop -->
          <div class="title pt-3">SHOP</div>
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
      <div class="footer-content-right"></div>
    </div>
    <!-- FOOTER BOTTOM -->

    <div class="footer-bottom content">
      <div class="sign">
        <button>SIGN-UP NOW!</button>
      </div>

      <div class="icons">
        <div class="px-4 text-primary fw-bold fs-4">FOLLOW US</div>
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
  </footer>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;

footer {
  background-color: #303030;
}

.content {
  @include margin_app();
}

.footer-top {
  @include footer_style();
  @include align_div();

  background-image: url(../assets/img/footer-bg.jpg);
  .footer-content-left {
    display: flex;
  }
  .footer-content-right {
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;

    width: 40rem;
    height: 20rem;
  }
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  padding-top: 2rem;
}
.icons {
  @include align_list();
  padding: 1rem 0;
}
button {
  @include button_hover();
}
</style>
