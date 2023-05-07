  <script>
  import comics from '../data/dc-comics.json';
  export default {
  name: 'myCard',
  props:{
    comic: Object
  },
  data(){
    return{
      comics
    }
  }
  }
  </script>

<template>
  <div class="card">
    <div class="image">
      <img :src="comic.thumb">
    </div>
    <div class="text">
      <h3>{{ comic.series }}</h3>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../scss/main.scss';
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
</style>