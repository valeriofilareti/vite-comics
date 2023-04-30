
<script>
import nav from '../data/nav-db.js';
export default {
  name: 'myHeader',
  data(){
    return {
      nav,
      isActive: true
    }
  },
  mounted(){

  }
}
</script>

<template>
  <header class="d-flex align-center">
    <div class="container d-flex align-center justify-between">
      <div class="logo d-flex align-center">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul class="d-flex">
          <li v-for="link in nav" :class="{ active: link.isActive }"><a href="">{{ link.name }}</a></li>


        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
  @use '../scss/main.scss';
  
  header {
    height: 100px;
    padding: 55px 0;
  }
  .logo {
    width: 80px;
  }
  .active {
    border-bottom: 5px solid red;
  }

  nav {
    height: 101px;
    line-height: 80px;
  }
    ul {
      li {
        padding: 10px;
        text-transform: uppercase;
        font-size: 12px;
      }

    }
  
</style>