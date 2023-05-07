
<script>
import comics from '../data/dc-comics.json';
import myCard from './myCard.vue';
export default {
  name: 'Main',
  data(){
    return {
      comics,
    }
  },
  components: {
    myCard
  },
  mounted(){
    
  }
}
</script>

<template>
  <main>
    <div class="container cards">
      <myCard
      v-for="(comic, index) in comics" :key="index" :comic="comic"
      />
      <!-- <div v-for="(comic, index) in comics" :key="index" class="card">
        <div class="image">
          <img :src="comic.thumb">
        </div>
        <div class="text">
          <h3>{{ comic.series }}</h3>
        </div>
      </div> -->
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../scss/main.scss';
  main {
    background-color: black;
    
  }
  h1 {
    color: white;
  }
  .card {
    width: 200px;
    padding: 10px;
    margin-top: 10px;
    .image{
      width: 180px;
      height: 180px;
      overflow: hidden;
    }
    .text {
      text-transform: uppercase;
      font-size: 12px;
      margin-top: 10px;
    }
  }
  .cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
</style>