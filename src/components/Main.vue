<template>
<div>
  <CoursesSection />
  <FacultiesSection />
</div>
</template>

<script>
import CoursesSection from './CoursesSection.vue'
import FacultiesSection from './FacultiesSection.vue'

export default {
  name: 'Main',
  components: {
    CoursesSection,
    FacultiesSection,
  }
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';
</style>
