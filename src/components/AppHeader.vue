<template>
  <section class="header">
    <div class="header__top"></div>
    <div class="header__bottom"></div>
  </section>
</template>

<script>
export default {
  name: "AppHeader",
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.header {
  width: 100%;

  &__top {
    background-color: $header-top-bg;
    height: $header-top-height;
  }

  &__bottom {
    background-image: $header-jumbotron-img;

    /*test*/
    height: 800px;
  }
}
</style>