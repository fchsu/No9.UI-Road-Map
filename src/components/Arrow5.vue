<template>
  <div>
    <canvas ref="arrow5"></canvas>
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
      const ctx = vm.$refs.arrow5.getContext('2d');
      vm.$refs.arrow5.width = 400;
      vm.$refs.arrow5.height = 400;
      ctx.beginPath();
        ctx.moveTo(20, 205);
        ctx.lineTo(35, 205);
        ctx.lineTo(35, 44);
        ctx.lineTo(20, 44);
        ctx.lineTo(20, 56);
        ctx.lineTo(0, 37);
        ctx.lineTo(20, 18);
        ctx.lineTo(20, 30);
        ctx.lineTo(65, 30);
        ctx.lineTo(65, 18);
        ctx.lineTo(85, 37);
        ctx.lineTo(65, 56);
        ctx.lineTo(65, 44);
        ctx.lineTo(55, 44);

        ctx.lineTo(55, 205);
        ctx.lineTo(90, 205);
        ctx.lineTo(90, 193);
        ctx.lineTo(110, 215);
        ctx.lineTo(90, 237);
        ctx.lineTo(90, 225);
        ctx.lineTo(55, 225);

        ctx.lineTo(55, 370);
        ctx.lineTo(65, 370);
        ctx.lineTo(65, 358);
        ctx.lineTo(85, 377);
        ctx.lineTo(65, 396);
        ctx.lineTo(65, 384);
        ctx.lineTo(20, 384);
        ctx.lineTo(20, 396);
        ctx.lineTo(0, 377);
        ctx.lineTo(20, 358);
        ctx.lineTo(20, 370);
        ctx.lineTo(35, 370);
        ctx.lineTo(35, 225);
        ctx.lineTo(20, 225);
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
