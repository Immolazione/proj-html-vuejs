<template>
<section id="header-jumbotron" class="position-relative">
  <div class="d-flex flex-column align-items-center container">
    <h1 class="text-center">Key to your success</h1>
    <p class="text-center">EduPrime is the most versitile WordPress theme for educational purposes, showcasing universities, courses, secondary schools etc.</p>
    <div>
      <button class="me-5 search-courses">Search Courses</button>
      <button class="ms-5 university-apply">Apply for university</button>
    </div>
  </div>
  <ul id="header-bookmarks" class="list-group position-absolute">
    <li class="list-group-item"></li>
    <li class="list-group-item"></li>
    <li class="list-group-item"></li>
  </ul>
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
  #header-bookmarks {
    top: 50%;
    transform: translate(0, -50%);
    padding: 0;
    border-radius: 0 10px 10px 0;
    li {
      padding: 0;
      border: $bg-color-yellow;
      background-color: $bg-color-yellow;
      height: 2rem;
      width: 2rem;
    }
  }
  * {
    padding: 2rem
  }
  .container {
    width: 50%;

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
        color: $text-color-white1;
        border: none;
        padding: 1rem 2rem;
        border-radius: 50px;
      }
      .search-courses {
        background-color: $bg-color-yellow;
        }
        .university-apply {
          background-color: $bg-color-white1;
          color: $text-color-red;
        }
    }
  }
  
}
</style>
