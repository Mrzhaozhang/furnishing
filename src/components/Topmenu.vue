<template>
	<div clas="top-menu">
		<div class="top-menu-nav">
			<div class="logo">
				<span></span>
				<span></span>
				<span></span>
			</div>
			<span class="menu-item" v-for="(item, index) in menu" :key="index" :class="{ active: activeIndex == index }">{{ item }}</span>
		</div>
	</div>
</template>

<script>
export default {
	name: 'topMenu',
	data() {
		return {
			menu: ['首页', '产品', '动态', '视频', '关于', '联系'],
			activeIndex: 0
		};
	},
	comments: {}
};
</script>

<style lang="less" scoped>
.top-menu-nav {
	margin: auto;
	width: 1220px;
	position: relative;
	text-align: right;
	height: 60px;
	line-height: 60px;
	.menu-item {
		color: rgba(0, 0, 0, 0.6);
		cursor: pointer;
		display: inline-block;
		width: 60px;
		font-size: 14px;
		transition: all .2s ease-in;
		&.active,&:hover{
			color: rgba(0, 0, 0, 1);
			font-size: 15px;
		}
	}
}
.logo{
	position: absolute;
	left: 0;
	top: 0;
	height: 100%;
	width: 24px;
	display: flex;
	align-items: center;
	cursor: pointer;
	span{
		display: inline-block;
		background: #333;
		height: 35%;
		width: 5px;
		margin-right: 4px;
		border-radius: 5px;
		transform:rotate(28deg)
	}
	&::after,&::before{
		content: '';
		position: absolute;
		height: 5px;
		width: 5px;
		background-color: #333;
		top: 21px;
		left: -5px;
		border-radius: 50%;
	}
	&::after{
		left: initial;
		right: -1px;
		top: initial;
		bottom: 20px;
	}
}
</style>
