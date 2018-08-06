<template>
  <div>
    <canvas ref="arrow3reverse"></canvas>
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
      const ctx = vm.$refs.arrow3reverse.getContext('2d');
      vm.$refs.arrow3reverse.width = 400;
      vm.$refs.arrow3reverse.height = 400;
      ctx.beginPath();
        ctx.moveTo(0, 185);
        ctx.lineTo(25, 185);
        ctx.lineTo(25, 50);
        ctx.lineTo(0, 50);
        ctx.lineTo(0, 30);
        ctx.lineTo(45, 30);
        ctx.lineTo(45, 185);

        ctx.lineTo(60, 185);
        ctx.lineTo(60, 173);
        ctx.lineTo(79, 195);
        ctx.lineTo(60, 217);
        ctx.lineTo(60, 205);
        ctx.lineTo(45, 205);

        ctx.lineTo(45, 365);
        ctx.lineTo(0, 365);
        ctx.lineTo(0, 345);
        ctx.lineTo(25, 345);
        ctx.lineTo(25, 205);
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
