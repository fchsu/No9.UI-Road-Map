<template>
  <div>
    <canvas ref="arrow3"></canvas>
  </div>
</template>

<script>
export default {
  data() {
    return {
      color: 'rgba(255, 255, 255, 0.33)',
      shadowColor: 'rgba(0, 147, 255, 0.35)',
    }
  },
  mounted() {
    this.draw(); 
  },
  methods: {
    draw() {
      const vm = this;
      const ctx = vm.$refs.arrow3.getContext('2d');
      vm.$refs.arrow3.width = 400;
      vm.$refs.arrow3.height = 400;
      ctx.beginPath();
        ctx.moveTo(0, 185);
        ctx.lineTo(20, 185);
        ctx.lineTo(20, 30);
        ctx.lineTo(57, 30);
        ctx.lineTo(57, 18);
        ctx.lineTo(74, 40);
        ctx.lineTo(57, 62);
        ctx.lineTo(57, 50);
        ctx.lineTo(40, 50);
        ctx.lineTo(40, 185);

        ctx.lineTo(57, 185);
        ctx.lineTo(57, 173);
        ctx.lineTo(74, 195);
        ctx.lineTo(57, 217);
        ctx.lineTo(57, 205);
        ctx.lineTo(40, 205);

        ctx.lineTo(40, 345);
        ctx.lineTo(57, 345);
        ctx.lineTo(57, 333);
        ctx.lineTo(74, 355);
        ctx.lineTo(57, 377);
        ctx.lineTo(57, 365);
        ctx.lineTo(20, 365);
        ctx.lineTo(20, 205);
        ctx.lineTo(0, 205);
      ctx.closePath();
      ctx.shadowBlur = 10;
      ctx.shadowColor = vm.shadowColor;
      ctx.fillStyle = vm.color;
      ctx.fill(); 
    }
  },
}
</script>

<style scoped lang="scss">
div {
  canvas {
    width: 100%;
    // border: 5px solid #000;
  }
}
</style>
