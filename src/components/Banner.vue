<template>
	<swiper class="banner-swiper" :options="swiperOption">
	   <swiper-slide>
		   <div class="slide-left">
			   <h3 class="title">北欧轻奢沙发</h3>
			   <p class="info">
				   全铜真皮现代轻奢精炼风格，选用意大利进口的特级牛皮，高级感扑面而来;精湛的车缝工艺不亚于爱马仕，精准地捕捉每-处优雅韵味，赋予了这款休闲沙发不一般的特质
			   </p>
			   <dl>
				   <dd>￥2680</dd>
				   <dd>立即购买</dd>
			   </dl>
		   </div>
		   <div class="slide-right">
		   			   
		   </div>
	   </swiper-slide>
	   <swiper-slide>Slide 2</swiper-slide>
	   <swiper-slide>Slide 3</swiper-slide>
	   <div class="swiper-pagination" slot="pagination"></div>
	 </swiper>
</template>

<script>
	export default{
		data(){
			return {
				swiperOption: {
				  direction: 'vertical',
				  loop : true,
				  // autoplay : {
				  //   delay:3000
				  // },
				  pagination: {
					el: '.swiper-pagination',
					clickable: true
				  }
				}
			}
		}
	}
</script>

<style lang="less" scoped>
	.banner-swiper{
		height: 100%;
		max-width: 1220px;
		width: 100%;
	}
	.swiper-slide{
		display: flex;
		align-items: center;
	}
	.slide-left,.slide-right{
		flex: 1;
		position: relative;
	}
	.slide-left	.title{
		text-align: left;
		font-weight: 600;
		font-size: 28px;
	}
	.slide-left	.info{
		font-size: 15px;
		text-align: left;
		margin-top: 50px;
		line-height: 30px;
	}
</style>
<style lang="less">
	.banner-swiper{
		.swiper-pagination {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
		}
		.swiper-pagination-bullet{
			width: 10px;
			height: 10px;
			border: 2px solid rgba(0,0,0,0);
			border-radius: 50%;
			background: none;
			position: relative;
			opacity: 1;
			transition: all .2s ease-in;
			background: none;
			&::after{
				content: '';
				width: 4px;
				height: 4px;
				border-radius: 50%;
				background: #333;
				position: absolute;
				left: 0;
				right: 0;
				top: 0;
				bottom: 0;
				margin: auto;
			}
		}
		.swiper-pagination-bullet-active{
			border: 2px solid rgba(0,0,0,1);
			background: #F4F4F4;
		}
	}
</style>
