<template>
  <section>
      <div id="faculties-description" class="container d-flex flex-column justify-content-center align-items-center">
        <h1>Faculties available at EduPrime</h1>
        <p class="text-center">A single university with a load of courses, tailored to satisfy any student's needs.</p>
      </div>
      <div id="faculties-tab">
        <div class="container">
          <div class="faculties-card position-relative d-flex justify-content-center align-items-center flex-column">
            <img src="../assets/img/Gavel-v2.png" alt="lax_faculty">
            <h3>Law Faculty</h3>
            <div class="position-absolute">&#9660;</div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'FacultiesSection'
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';

#faculties-description {
  h1 {
    font-family: $itim;
  }
  p {
    width: 40%;
  }
}
#faculties-tab {
  height: 10rem;
  box-shadow: 0 0 5px 0px $border-color-grey4;
  .position-absolute {
    top: 96%;
    left: 50%;
    transform: translate(-50%);
    color: $bg-color-red1;
  }
}
.faculties-card {
  width: calc(100% / 5);
  height: 10rem;
  background-color: $bg-color-red1;
  border-left: 1px solid $border-color-grey4;
  border-right: 1px solid $border-color-grey4;
  img{
    height: 60%;
    color: $text-color-white1;
  }
  h3 {
    font-family: $itim;
    color: $text-color-white1;
  }
}
</style>