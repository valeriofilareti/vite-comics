
<script>
export default {
  name: 'myHeader'
}
</script>

<template>
  <header class="d-flex align-center">
    <div class="container d-flex align-center justify-between">
      <div class="logo d-flex align-center">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
          <li><a href="">link</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
  @use '../scss/main.scss';
  
  header {
    height: 100px;
    border: 1px solid black;
  }
  .logo {
    width: 80px;
  }

  nav {
    ul {
      display: flex;
      li {
        padding: 10px;
      }
    }
  }
</style>