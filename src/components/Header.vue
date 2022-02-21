<template>
<section class="header-layer">
  <section class="header-bg">
  <HeaderNavigation />
  <HeaderJumbotron />
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
    height: 700px;
    .header-bg {
      height: 100%;
      opacity: 0.1;
      // filter: grayscale(100%); PROB BUONA PROPRIETà
      background-color: $bg-color-red1;
      background-image: url(../assets/img/theme_slider2_bg-1.jpg);
      background-repeat: no-repeat;
      background-position: center;
      background-size: cover;
    }
  }
</style>
