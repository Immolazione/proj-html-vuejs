<template>
<section id="header-navbar" class="d-flex justify-content-between">
  <img src="../assets/img/theme_eduprime_logo.png" alt="Header_Logo">
  <div class="d-flex align-items-center">
    <ul class="d-flex align-items-center">
      <li><a href="#">Home</a><span>&#x25BE;</span></li>
      <li><a href="#">Courses</a><span>&#x25BE;</span></li>
      <li><a href="#">About Us</a><span>&#x25BE;</span></li>
      <li><a href="#">News</a><span>&#x25BE;</span></li>
      <li><a href="#">Pages</a><span>&#x25BE;</span></li>
      <li><a href="#">Contact</a></li>
      <li><a href="#">Purchase</a></li>
    </ul>
    <button type="button">VIEW COURSES</button>
  </div>
</section>  
</template>

<script>

export default {
  name: 'HeaderNavigation',
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';

#header-navbar {
  img {
    height: 5rem;
    margin: 2rem;
  }
  div{
    margin-right: 4rem;
    ul {
      margin: 0;
      padding: 0;
      li {
        list-style-type: none;
        padding: 0 1.5rem;
        a {
          font-family: $itim;
          text-decoration: none;
          color: $text-color-white1;
        }
        span {
          color: $text-color-white1;
      }
    }
  }
    button{
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
