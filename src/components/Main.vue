<template>
<div>
  <CoursesSection />
  <FacultiesSection />
  <AcademicYear />
</div>
</template>

<script>
import CoursesSection from './CoursesSection.vue'
import FacultiesSection from './FacultiesSection.vue'
import AcademicYear from './AcademicYear.vue'

export default {
  name: 'Main',
  components: {
    CoursesSection,
    FacultiesSection,
    AcademicYear
  }
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';
</style>
