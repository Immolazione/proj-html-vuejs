<template>
<section id="header-jumbotron" class="position-relative">
  <div class="d-flex flex-column align-items-center container">
    <h1>Key to your success</h1>
    <p>EduPrime is the most versitile WordPress theme for educational purposes, showcasing universities, courses, secondary schools etc.</p>
    <div>
      <button class="me-5">Search Courses</button>
      <button class="ms-5">Apply for university</button>
    </div>
  </div>
</section>
</template>

<script>

export default {
  name: 'HeaderJumbotron',
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';

#header-jumbotron {
  * {
    padding: 2rem
  }
  h1 {
    color: $text-color-white1;
    font-size: 4rem;
    font-family: $itim;
  }
  p {
    color: $text-color-white1;
  }
  div {
    button { // MEGLIO LUNGHEZZA UGUALE PER COERENZA
      font-family: $itim;
      background-color: $bg-color-yellow;
      color: $text-color-white1;
      border: none;
      padding: 1rem;
      border-radius: 50px;
    }
  }
}
</style>
