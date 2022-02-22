<template>
<section class="header-bg">
  <section class="header-layer position-relative">
    <HeaderNavigation :navbar="navbar" />
    <HeaderJumbotron />
    <img src="../assets/img/Wave-1.png" class="w-100" alt="wave">
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
  },
  data() {
    return{
      navbar: [{name: 'Home', arrow: true},
      {name: 'Courses', arrow: true},
      {name: 'About Us', arrow: true},
      {name: 'News', arrow: true},
      {name: 'Pages', arrow: true},
      {name: 'Contact', arrow: false},
      {name: 'Purchase', arrow: false},]
    }
  }

}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';

  .header-layer{
    background-color: $bg-color-red2;
    height: 800px;
  }
  .header-bg {
  // opacity: 0.1;
    height: 100%;
    // filter: grayscale(100%); PROB BUONA PROPRIETà
    // background-color: $bg-color-red1;
    background-image: url(../assets/img/theme_slider2_bg-1.jpg);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;

  }
  img {
    position: absolute;
    bottom: 0;
  }
</style>
