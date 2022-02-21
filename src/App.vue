<template>
<section>
  <Header />
  <Main />
  <Footer />
</section>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss" scoped>
@import './assets/scss/style.scss';

</style>
