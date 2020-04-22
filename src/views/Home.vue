<template>
  <div class="home">
    <div class="banner">
		<Banner></Banner>
	</div>
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue'

export default {
  name: 'Home',
  components: {
	Banner
  }
}
</script>
<style lang="less" scoped>
	.banner{
		height: 500px;
		background: #F4F4F4;
	}
</style>
