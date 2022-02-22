<template>
  <section class="position-relative">
    <div id="faculties-title" class="container d-flex flex-column justify-content-center align-items-center">
      <h1>Faculties available at EduPrime</h1>
      <p class="text-center">A single university with a load of courses, tailored to satisfy any student's needs.</p>
    </div>
    <div id="faculties-tab">
        <div class="container d-flex">
          <div class="faculties-card position-relative d-flex justify-content-center align-items-center flex-column">
            <img src="../assets/img/Gavel-v2.png" alt="law_faculty">
            <h3>Law Faculty</h3>
            <!-- <div class="position-absolute">&#9660;</div> -->
          </div>
          <div class="faculties-card position-relative d-flex justify-content-center align-items-center flex-column">
            <img src="../assets/img/Coins-tabs-v2.png" alt="economy_faculty">
            <h3>Economy</h3>
            <!-- <div class="position-absolute">&#9660;</div> -->
          </div>
          <div class="faculties-card position-relative d-flex justify-content-center align-items-center flex-column">
            <img src="../assets/img/Medicine-tabs-v2.png" alt="medicine_faculty">
            <h3>Medicine</h3>
            <!-- <div class="position-absolute">&#9660;</div> -->
          </div>
          <div class="faculties-card position-relative d-flex justify-content-center align-items-center flex-column">
            <img src="../assets/img/Computer-tabs-v2.png" alt="computer_science_faculty">
            <h3>Computer Science</h3>
            <!-- <div class="position-absolute">&#9660;</div> -->
          </div>
          <div class="faculties-card position-relative d-flex justify-content-center align-items-center flex-column">
            <img src="../assets/img/Palette-tabs-v2.png" alt="design_faculty">
            <h3>Graphic Design</h3>
            <!-- <div class="position-absolute">&#9660;</div> -->
          </div>
        </div>
    </div>
    <div id="faculties-tab-description" class="container">
      <div class="row">
        <div class="col-5 offset-1">
          <img src="../assets/img/Gavel-Illustration-e1556884768193.png" alt="law-faculty">
        </div>
        <div class="col-5">
          <h1>Law Faculty</h1>
          <p>Learning from world-leading academics and practitioners, you'll not only receive an outstanding groundind in the theory of law, but you will be able to understand how those principles are applied in practice through a range of student-led activities and competitions</p>
          <button>Read More</button>
        </div>
      </div>
    </div>
    <div class="position-absolute">
     <svg class="w-100" version="1.0" xmlns="http://www.w3.org/2000/svg" width="2954.667" height="186.667" viewBox="0 0 2216 140"><path class="st0" d="M324.7 34.8c-76.4 51.8-134.1 82-177.2 92.8-12.2 3.1-33.8 4.3-42.8 2.5-8.1-1.7-18.5-7.2-24.2-12.8-5.7-5.7-10.1-12.2-17.4-26.1C57 79.6 52.6 75 47.7 75c-7.9 0-21.2 9.9-37.9 28.3L0 114v26h1105.2c729.3 0 1104.9-.3 1104.2-1-2.6-2.6-29.5-18-42.9-24.5-46.4-22.7-82.1-27.7-122.7-17.5-4.6 1.2-19.1 5.5-32.3 9.5-40.2 12.4-58.5 16.1-85.5 17.2-33.9 1.3-73.5-5.3-117.9-19.9-14.8-4.8-48.5-17.8-59.7-23l-5.2-2.4-16.3 1.8c-125.9 13.6-219.6 20.5-324.9 23.9-40.1 1.3-166.2.6-196-1-71.9-4-119.7-8.4-173.5-16.2-26.8-3.8-69.6-11.2-83.1-14.4-5-1.1-8-1.3-13.2-.5-3.7.5-18.8 2.3-33.7 3.9C793 88.1 702 89.1 622 79c-51.2-6.5-89.6-15.2-150.5-34-35.4-10.9-84.3-20.7-121.8-24.3-3.5-.3-5.6.9-25 14.1z" fill="#e56768"/></svg>
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

section {
  height: 750px;
}
section > .position-absolute {
  top: 80%;
}
#faculties-title {
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
  border-left: 1px solid $border-color-grey4;
  border-right: 1px solid $border-color-grey4;
  img{
    height: 60%;
  }
  h3 {
    font-family: $itim;
    color: $text-color-red;
  }
}
#faculties-tab-description {
  margin-top: 5rem;
  h1{
    font-family: $itim;
  }
  button {
    font-family: $itim;
    color: $text-color-white1;
    background-color: $bg-color-red1;
    border: none;
    padding: 1rem 2rem;
    border-radius: 50px;
  }
}
</style>