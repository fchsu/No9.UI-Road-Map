<template>
  <div>
    <canvas ref="arrow2in1"></canvas>
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
      const ctx = vm.$refs.arrow2in1.getContext('2d');
      ctx.beginPath();
        ctx.moveTo(0, 18);
        ctx.lineTo(55, 18);
        ctx.lineTo(55, 82);
        ctx.lineTo(110, 82);
        ctx.lineTo(110, 65);
        ctx.lineTo(135, 92);
        ctx.lineTo(110, 119);
        ctx.lineTo(110, 102);
        ctx.lineTo(55, 102);
        ctx.lineTo(55, 138);
        ctx.lineTo(35, 138);
        ctx.lineTo(35, 38);
        ctx.lineTo(0, 38);
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
