<template>
  <div>
    <canvas ref="arrow1"></canvas>
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
      const ctx = vm.$refs.arrow1.getContext('2d');
      ctx.beginPath();
        ctx.moveTo(0, 18);
        ctx.lineTo(38, 18);
        ctx.lineTo(38, 0);
        ctx.lineTo(75, 30);
        ctx.lineTo(38, 60);
        ctx.lineTo(38, 42);
        ctx.lineTo(0, 42);
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
