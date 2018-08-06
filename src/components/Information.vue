<template>
	<div id="information">
		<ul class="info">
			<li class="d-flex">
				<div class="img_skill"></div>
        <div class="message">
          <p class="title">安安</p>
          <p class="mb-3">我是Mono喵，接下來將你領略UI的變換。喵。</p>
        </div>
			</li>
		</ul>
		<div class="img"></div>
	</div>
</template>

<script>
export default {
  
}
</script>


<style scoped lang="scss">
	#information {
    width: 1440px;
    @media (max-width: 1440px) {
      width: 100%;
    }
		height: 0;
    padding-top: 15%;
    margin: 0 auto;
		position: relative;
		.img {
			width: 13%;
			height: 0;	
      padding-top: 22%;
			background: url('../assets/img/img_monocat.png') 50% 50% no-repeat;
			background-size: cover;
			position: absolute;
			top: 0;
      left: 0;
      @media (max-width: 1440px) {
        width: 13vw;
        padding-top: 19vw;
      }
		}
		.info {
			width: 75%;
			position: absolute;
			top: 13%;
			left: 9.2%;
      margin: 0;
      padding: 0;
			li {
				border: 8px solid #0093FF;
				border-radius: 60px;
				@media (max-width: 1440px) {
					border: 0.5vw solid #0093FF;
          border-radius: 4.3vw;
				}
				background: #FFF;
        .img_skill {
          width: 15%;
          height: 0;
          padding-top: 15%;
          margin-left: 6%;
          margin-top: 32px;
          @media (max-width: 1440px) {
            margin-top: 1.9vw;
          }
        }
        .message {
          min-height: 220px;
          padding-top: 22px;
          margin-left: -5%;
          @media (max-width: 1440px) {
            min-height: 13vw;
            padding-top: 1.5vw;
          }
          p {
            margin-bottom: 0px;
            font-size: 2rem * 1.1;
            transform: scale(0.8);
            @media (max-width: 1440px) {
              font-size: 2vw * 1.25;
            }
            font-family: $skill-tree, $font-family-base;
          }
          .title {
            font-weight: bold;
          }
        }
			}
		}
	}
</style>