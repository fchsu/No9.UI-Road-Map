<template>
  <div id="home" class="container">
    <div class="row align-items-center mb-5">
      <div class="logo1">
        <div class="logo2">
          <div class="logo3"></div>
        </div>
      </div>
      <h1 class="d-flex flex-column">
        <span class="h1-cht">介面設計師轉職之路</span>
        <span class="h1-eng">UI Designer Road Map</span>
      </h1>
    </div>
    <SkillTree></SkillTree>
    <!-- <Information></Information> -->
  </div>
</template>

<script>
import SkillTree from '../SkillTree';
// import Information from '../Information';
export default {
  name: 'HomePage',
  data () {
    return {
      
    }
  },
  components: {
    SkillTree,
    // Information,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#home {
  max-width: 1440px;
  height: 100%;
  padding-top: 5%;
  .logo1 {
    width: 13%;
    height: 0;
    padding-top: 13%;
    position: relative;
    margin-right: 5vw;
    background: url('../../assets/img/img_illustration@2x.png') 50% 50% no-repeat;
    background-size: 70% 70%;
    @media (max-width: 1600px) {
      margin-left: 5vw;
    }
    .logo2 {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      background-color: rgba(239, 190, 171, .3);
      position: absolute;
      top: 0;
      left: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      .logo3 {
        width: 85%;
        height: 85%;
        border-radius: 50%;
        background-color: rgba(239, 190, 171, .6);
      }
    }
  }
  h1 {
    color: #FFF;
    .h1-cht {
      font-family: $h1-cht, $font-family-base;
      font-weight: bold;
      font-size: 5rem;
    }
    .h1-eng {
      font-family: $h1-eng, $font-family-base;
      font-weight: bold;
      font-size: 5rem;
    }
    @media (max-width: 1440px) {
      .h1-cht, .h1-eng {
        font-size: 5vw;
      }
    }
  }
}
</style>
