
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
                <h2>{{ linksMenu[0].name }}</h2>
                <li v-for="link in linksMenu[0].links"><a href="#">{{link}}</a></li>
              </ul>
              <ul>
                <h2>{{ linksMenu[1].name }}</h2>
                <li v-for="link in linksMenu[1].links"><a href="#">{{link}}</a></li>
              </ul>
            </ul>
          </div>
          <div class="col">
            <ul>
              <h2>{{ linksMenu[2].name }}</h2>
                <li v-for="link in linksMenu[2].links"><a href="#">{{link}}</a></li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <h2>{{ linksMenu[3].name }}</h2>
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
  h2 {
    color: #d0d0d0;
    text-transform: uppercase;
    margin: 20px 0;
  }
  .footer-top {

    .col {
      padding: 10px;
      ul {
        margin: 0 10px;
      }
      li {
        margin: 5px 0;
        font-size: 12px;
        text-transform: capitalize;
        color: rgb(184, 29, 29);
      }
      
    }
    a {
      color: grey
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
  .footer-links {
    padding: 15px;
  }

</style>