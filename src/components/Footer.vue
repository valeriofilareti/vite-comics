
<script>
export default {
  name: 'Footer'
}
</script>

<template>
  <footer>
    <div class="container">
      <div class="footer-top d-flex justify-between">
        <div class="footer-links d-flex">
          <div class="col">
            <ul>
              <li><h2>link</h2></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <li><h2>link</h2></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <li><h2>link</h2></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
              <li><a href="#">link</a></li>
            </ul>
          </div>
          <div class="col"></div>
          <div class="col"></div>
        </div>
        <div class="footer-img">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
    <div class="footer-bottom"></div>
  </footer>
</template>

<style lang="scss" scoped>
  @use '../scss/main.scss';

  footer {
    background-image: url(../assets/img/footer-bg.jpg);
  }
  .footer-top {
    height: 350px;

    .col {
      padding: 10px;
      li {
        margin: 5px 0;
      }
      
    }
    a {
      color: white;
    }
  }
  .footer-bottom {
    height: 80px;
    background-color: gray;
  }

  .footer-img {
    width: 500px;
    overflow: hidden;
  }
</style>