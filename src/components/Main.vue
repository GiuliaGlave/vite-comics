<script></script>

<template>
  <div class="container">
    <div class="content">-->Content goes here--</div>

    <div class="section">
      <ul>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
        <li><a href="#">link</a></li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins.scss" as *;
.section {
  @include align_li();
  @include bottom_section();
}

.content {
  background-color: #1c1c1c;
  color: white;
  padding: 2rem 0;
}
</style>
