
<script>
import nav from '../data/nav-db.js';
export default {
  name: 'myHeader',
  data(){
    return {
      nav,
      isActive: true,
      counter: ''
    }
  },
  methods: {
    addActive(){
      count++;
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
          <li 
            v-for="(link, index) in nav" 
            :class="{ active: counter === index }" 
            @click="counter = index" 
            :key="index">
            <a href="#">{{ link.name }}</a>
          </li>
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
    border-bottom: 5px solid rgb(43, 0, 255);
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
        a {
          color: black;
        }
      }

    }
  
</style>


<!-- <a href="">{{ link.name }}</a> -->