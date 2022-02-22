<template>
<section id="header-navbar" class="d-flex justify-content-between">
  <img src="../assets/img/theme_eduprime_logo.png" alt="Header_Logo">
  <div class="d-flex align-items-center">
    <ul class="d-flex align-items-center">
      <li class="nav-item" v-for="(item, index) in navbar" :key="index">
        <a class="nav-item" href="#">{{ item.name }}
          <span class="ms-1 nav-item" v-if="item.arrow">&#x25BE;</span>
        </a>
      </li>

    </ul>
    <button type="button">VIEW COURSES</button>
  </div>
</section>  
</template>

<script>

export default {
  name: 'HeaderNavigation',
  props: ['navbar']
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
        .nav-item:hover {
          color: $text-color-yellow;
        }   
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
      padding: 1rem 2rem;
      border-radius: 50px;
    }
    button:hover{
      background-color: $bg-color-white1;
      color: $text-color-red;
    }
  }
}

</style>
