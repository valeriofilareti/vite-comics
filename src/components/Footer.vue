
<script>
import linksMenu from '../data/footer-db'
export default {
  name: 'Footer',
  data(){
    return {
      linksMenu
    }
  }
}
</script>

<template>
  <footer>
    <div class="container">
      <div class="footer-top d-flex justify-between">
        <div class="footer-links d-flex">
          <div class="col">
            <ul>
              <ul>
                <li><h2>{{ linksMenu[0].name }}</h2></li>
                <li v-for="link in linksMenu[0].links"><a href="#">{{link}}</a></li>
              </ul>
              <ul>
                <li><h2>{{ linksMenu[1].name }}</h2></li>
                <li v-for="link in linksMenu[1].links"><a href="#">{{link}}</a></li>
              </ul>
            </ul>
          </div>
          <div class="col">
            <ul>
              <li><h2>{{ linksMenu[2].name }}</h2></li>
                <li v-for="link in linksMenu[2].links"><a href="#">{{link}}</a></li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <li><h2>{{ linksMenu[3].name }}</h2></li>
                <li v-for="link in linksMenu[3].links"><a href="#">{{link}}</a></li>
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
    position: relative;
    img {
      position: absolute;
      bottom: -65px;
    }
  }

</style>