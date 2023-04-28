
<script>
import myHeader from './components/myHeader.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';
import Jumbo from './components/Jumbo.vue';


export default {
  name: 'App',
  components: {
    myHeader,
    Main,
    Footer,
    Jumbo
  },
  data(){
    return {
      title: 'dc-vite',
      
    }
  },
  mounted() {
    console.log(this.comics);
  }
}
</script>
<template>
  <myHeader />
  <Jumbo />
  <Main />
  <Footer />

</template>

<style lang="scss">
  @use './scss/general/general.scss';
  

</style>