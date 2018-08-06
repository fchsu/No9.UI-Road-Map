<template>
  <div id="app">
    <router-view/>
    <div class="back-img">
      <div class="rocket"></div>
      <div class="backImage"></div>
      <div class="hexcat"></div>
      <div class="information">
        <Information></Information>
      </div>
    </div>
  </div>
</template>

<script>
import Information from './components/Information';
export default {
  name: 'App',
  components: {
    Information,
  },
}
</script>

<style lang="scss">
@import './assets/all';
#app {
  min-height: 100vh;
  background-color: #301A3B;
  .back-img {
    width: 100%;
    // border: 1px solid #fff;
    overflow: hidden;
    position: relative;
    .backImage {
      padding-top: 57%;
      background: url('./assets/img/img_footer.png') no-repeat;
      background-size: cover;
      transform: translateY(14%);
    }
    .hexcat {
      width: 16vw;
      height: 16vw * 1.07;
      background: url('./assets/img/img_hexcat.png') no-repeat 50% 50%;
      background-size: cover;
      position: absolute;
      bottom: 23%;
      left: 3.3%;
    }
    .rocket {
      width: 13vw;
      height: 13vw * 2.76;
      background: url('./assets/img/img_rocket.png');
      background-size: cover;
      position: absolute;
      bottom: -2%;
      right: 16.2%;
    }
    .information {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      @media (max-width: 1440px) {
        width: 95vw;
      }
    }
  }
}
</style>
