
<script>
import myHeader from './components/myHeader.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';
import comics from './data/dc-comics.json';

export default {
  name: 'App',
  components: {
    myHeader,
    Main,
    Footer
  },
  data(){
    return {
      title: 'dc-vite',
      comics
    }
  },
  mounted() {
    console.log(this.comics);
  }
}
</script>
<template>
  <myHeader />
  <Main />
  <Footer />

</template>

<style lang="scss">
  @use './scss/general/general.scss';
  

</style>