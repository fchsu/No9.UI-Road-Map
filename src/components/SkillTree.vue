<template>
  <div class="mb-5" id="skill">
    <Arrow1_1 id="arrow1-1"></Arrow1_1>
    <Arrow1_2 id="arrow1-2"></Arrow1_2>
    <Arrow1_3 id="arrow1-3"></Arrow1_3>
    <Arrow1_4 id="arrow1-4"></Arrow1_4>
    <Arrow2in1 id="arrow2in1"></Arrow2in1>
    <Arrow3 id="arrow3"></Arrow3>
    <Arrow3Reverse id="arrow3reverse"></Arrow3Reverse>
    <Arrow5 id="arrow5"></Arrow5>

    <div class="skill-box-outside img_blade-1">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img" :style="{ backgroundImage: 'url(' + require('../assets/img/img_blade-1.png') + ')' }"></div>
      <p class="text-light">設計規範</p>
    </div>
    <div class="skill-box-outside img_meat">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img" :style="{ backgroundImage: 'url(' + require('../assets/img/img_meat.png') + ')' }"></div>
      <p class="text-light">爬梳乾貨</p>
    </div>
    <div class="skill-box-outside img_shield">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img shield" :style="{ backgroundImage: 'url(' + require('../assets/img/img_shield.png') + ')' }"></div>
      <p class="text-light text-shift">UX思維</p>
    </div>
    <div class="skill-box-outside img_hat">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img hat" :style="{ backgroundImage: 'url(' + require('../assets/img/img_hat.png') + ')' }"></div>
      <p class="text-light">設計思考</p>
    </div>
    <div class="skill-box-outside img_horn">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img horn" :style="{ backgroundImage: 'url(' + require('../assets/img/img_horn.png') + ')' }"></div>
      <p class="text-light text-shift-3ch">心理學</p>
    </div>
    <div class="skill-box-outside img_hammer">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img hammer" :style="{ backgroundImage: 'url(' + require('../assets/img/img_hammer.png') + ')' }"></div>
      <p class="text-light text-shift-3ch">線框稿</p>
    </div>
    <div class="skill-box-outside img_illustration">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img illustration" :style="{ backgroundImage: 'url(' + require('../assets/img/img_illustration.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">插畫</p>
    </div>
    <div class="skill-box-outside img_color">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img color" :style="{ backgroundImage: 'url(' + require('../assets/img/img_color.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">配色</p>
    </div>
    <div class="skill-box-outside img_sense">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img" :style="{ backgroundImage: 'url(' + require('../assets/img/img_sense.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">美感</p>
    </div>
    <div class="skill-box-outside img_text">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img text" :style="{ backgroundImage: 'url(' + require('../assets/img/img_text.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">文案</p>
    </div>
    <div class="skill-box-outside img_inspiration">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img inspiration" :style="{ backgroundImage: 'url(' + require('../assets/img/img_inspiration.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">靈感</p>
    </div>
    <div class="skill-box-outside img_pictures">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img pictures" :style="{ backgroundImage: 'url(' + require('../assets/img/img_pictures.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">圖庫</p>
    </div>
    <div class="skill-box-outside img_axe">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img axe" :style="{ backgroundImage: 'url(' + require('../assets/img/img_axe.png') + ')' }"></div>
      <p class="text-light text-shift">UI設計</p>
    </div>
    <div class="skill-box-outside img_blade">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img" :style="{ backgroundImage: 'url(' + require('../assets/img/img_blade.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">原型</p>
    </div>
    <div class="skill-box-outside img_book">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img book" :style="{ backgroundImage: 'url(' + require('../assets/img/img_book.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">標註</p>
    </div>
    <div class="skill-box-outside img_quill">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img quill" :style="{ backgroundImage: 'url(' + require('../assets/img/img_quill.png') + ')' }"></div>
      <p class="text-light">略懂開發</p>
    </div>
    <div class="skill-box-outside img_sword">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img sword" :style="{ backgroundImage: 'url(' + require('../assets/img/img_sword.png') + ')' }"></div>
      <p class="text-light text-shift-2ch">出師</p>
    </div>
    <div class="skill-box-outside img_timer">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img timer" :style="{ backgroundImage: 'url(' + require('../assets/img/img_timer.png') + ')' }"></div>
      <p class="text-light">版本控制</p>
    </div>
    <div class="skill-box-outside img_emblem">
      <div class="skill-box-inside1"></div>
      <div class="skill-box-inside2"></div>
      <div class="img emblem" :style="{ backgroundImage: 'url(' + require('../assets/img/img_emblem.png') + ')' }"></div>
      <p class="text-light text-shift-3ch">厚黑學</p>
    </div>
  </div>
</template>

<script>
import Arrow1_1 from './Arrow1_1';
import Arrow1_2 from './Arrow1_2';
import Arrow1_3 from './Arrow1_3';
import Arrow1_4 from './Arrow1_4';
import Arrow2in1 from './Arrow2in1';
import Arrow3 from './Arrow3';
import Arrow3Reverse from './Arrow3Reverse';
import Arrow5 from './Arrow5';

export default {
  name: 'SkillTree',
  data () {
    return {

    }
  },
  components: {
    Arrow1_1,
    Arrow1_2,
    Arrow1_3,
    Arrow1_4,
    Arrow2in1,
    Arrow3,
    Arrow3Reverse,
    Arrow5,
  },
}
</script>

<style scoped lang="scss">
#skill {
  position: relative;
  height: 0;
  padding-top: 42%;
  // border: 1px solid #fff;
  overflow: hidden;
  #arrow1-1 {
    width: 20%;
    position: absolute;
    top: 29%;
    left: 7.5%;
  }
  #arrow1-2 {
    width: 20%;
    position: absolute;
    top: 59%;
    left: 7%;
  }
  #arrow1-3 {
    width: 20%;
    position: absolute;
    top: 59%;
    left: 17.8%;
  }
  #arrow1-4 {
    width: 20%;
    position: absolute;
    top: 41%;
    left: 73.2%;
  }
  #arrow2in1 {
    width: 25%;
    position: absolute;
    top: 27.5%;
    left: 21%;
  }
  #arrow3 {
    width: 31%;
    position: absolute;
    top: 11%;
    left: 39.2%;
  }
  #arrow3reverse {
    width: 31%;
    position: absolute;
    top: 11%;
    left: 60%;
  }
  #arrow5 {
    width: 31%;
    position: absolute;
    top: 6.5%;
    left: 83.7%;
  }
  .skill-box-outside {
    width: 7%;
    padding-top: 7%;
    background: rgba(92, 92, 92, 0.62);
    border-radius: 40%;
    position: relative;
    cursor: pointer;
    .skill-box-inside1 {
      width: 86%;
      height: 86%;
      background: rgba(81, 93, 119, 0.75);
      border-radius: 40%;
      box-shadow: 0 0 0.375rem rgba(81, 93, 119, 0.64);
      position: absolute;
      top: 7%;
      left: 7%;
    }
    .skill-box-inside2 {
      width: 72%;
      height: 72%;
      background-color: rgba(0, 147, 255, 0.35);
      border-radius: 40%;
      box-shadow: 0 0 0.375rem rgba(0, 147, 255, 0.44);
      position: absolute;
      top: 14%;
      left: 14%;
    }
    .img {
      width: 80%;
      height: 80%;
      background-position: 50% 50%;
      background-repeat: no-repeat;
      background-size: contain;
      position: absolute;
      top: 10%;
      left: 10%;
      &.shield, {
        width: 66%;
        height: 66%;
        top: 17%;
        left: 10%;
      }
      &.hat, .horn, .hammer, .book, .quill, .timer, {
        width: 90%;
        height: 90%;
        top: 5%;
        left: 5%;
      }
      &.illustration, .text {
        width: 56%;
        height: 56%;
        top: 22%;
        left: 22%;
      }
      &.color {
        width: 50%;
        height: 50%;
        top: 25%;
        left: 25%;
      }
      &.inspiration {
        width: 60%;
        height: 60%;
        top: 20%;
        left: 18%;
      }
      &.pictures {
        width: 53%;
        height: 53%;
        top: 15%;
        left: 20%;
      }
      &.axe {
        width: 90%;
        height: 90%;
        top: 10%;
        left: 5%;
      }
      &.sword {
        width: 120%;
        height: 120%;
        top: -17%;
        left: -6%;
      }
      &.emblem {
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
      }
    }
    p {
      position: absolute;
      bottom: -42%;
      left: 0;
      font-family: $skill-tree, $font-family-base;
      font-weight: bold;
      font-size: 1.5rem;
      transform: scale(0.8);
      margin: 0 0 0 2.5%;
      text-align: center;
      &.text-shift {
        margin: 0 0 0 10%;
      }
      &.text-shift-3ch {
        margin: 0 0 0 14%;
      }
      &.text-shift-2ch {
        margin: 0 0 0 26%;
      }
      @media (max-width: 1440px) {
        font-size: 1.6vw;
      }
      @media (max-width: 600px) {
        margin: 0;
      }
    }
  }
  .img_blade-1 {
    position: absolute;
    top: 25%;
    left: 0;
  }
  .img_meat {
    position: absolute;
    top: 25%;
    left: 14%;
  }
  .img_shield {
    position: absolute;
    top: 55%;
    left: 0;
  }
  .img_hat {
    position: absolute;
    top: 55%;
    left: 10.8%;
  }
  .img_horn {
    position: absolute;
    top: 55%;
    left: 21.2%;
  }

  .img_hammer {
    position: absolute;
    top: 38%;
    left: 32.2%;
  }
  .img_illustration {
    position: absolute;
    top: 10%;
    left: 45%;
  }
  .img_color {
    position: absolute;
    top: 10%;
    left: 53%;
  }
  .img_sense {
    position: absolute;
    top: 39%;
    left: 45%;
  }
  .img_text {
    position: absolute;
    top: 39%;
    left: 53%;
  }
  .img_inspiration {
    position: absolute;
    top: 68%;
    left: 45%;
  }
  .img_pictures {
    position: absolute;
    top: 68%;
    left: 53%;
  }

  .img_axe {
    position: absolute;
    top: 37%;
    right: 26.8%;
  }
  .img_blade {
    position: absolute;
    top: 38%;
    right: 14.8%;
  }
  .img_book {
    position: absolute;
    top: 4%;
    right: 16.6%;
  }
  .img_quill {
    position: absolute;
    top: 2%;
    right: 2.4%;
  }
  .img_sword {
    position: absolute;
    top: 37%;
    right: 0;
  }
  .img_timer {
    position: absolute;
    top: 68%;
    right: 16.8%;
  }
  .img_emblem {
    position: absolute;
    top: 69.5%;
    right: 2.6%;
  }
}
</style>
