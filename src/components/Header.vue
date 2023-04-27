
<script>
export default {
  name: 'Header'
}
</script>

<template>
  <header>
    
    <div class="logo">
      <img src="../assets/img/dc-logo-bg.png" alt="">
    </div>
    <nav></nav>
  </header>
</template>

<style lang="scss" scoped>
  @use '../scss/main.scss';
  
  header {
    height: 100px;
    border: 1px solid black;
  }
  .logo {
    width: 50px;
  }
</style>