<template>
<section class="header-layer">
  <section class="header-bg position-relative">
    <HeaderNavigation />
    <HeaderJumbotron />
    <img src="../assets/img/Wave-1.png" alt="wave">
  </section>
</section>
</template>

<script>
import HeaderNavigation from './HeaderNavigation.vue'
import HeaderJumbotron from './HeaderJumbotron.vue'

export default {
  name: 'Header',
  components: {
    HeaderNavigation,
    HeaderJumbotron
  }
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';

  .header-layer{
    background-color: $bg-color-red1;
    height: 800px;
    .header-bg {
      // opacity: 0.1;
      height: 100%;
      // filter: grayscale(100%); PROB BUONA PROPRIETà
      // background-color: $bg-color-red1;
      // background-image: url(../assets/img/theme_slider2_bg-1.jpg);
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover;
      img {
        position: absolute;
        bottom: 0;
      }
    }
  }
</style>
