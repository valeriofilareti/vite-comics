
<script>
import comics from '../data/dc-comics.json';
export default {
  name: 'Main',
  data(){
    return {
      comics
    }
  },
  mounted(){
    
  }
}
</script>

<template>
  <main>
    <div class="container cards">
      <div v-for="comic in comics" class="card">
        <div class="image">
          <img :src="comic.thumb">
        </div>
        <div class="text">
          <h3>{{ comic.series }}</h3>
        </div>
      </div>
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
    .image{
      width: 180px;
      height: 180px;
      border: 1px solid red;
      overflow: hidden;
    }
  }

  .cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
</style>