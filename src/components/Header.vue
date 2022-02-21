<template>
<section>
 <HeaderNavigation />
 <HeaderJumbotron />
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
</style>
