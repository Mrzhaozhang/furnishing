<template>
  <div class="home">
    <div class="banner">
		
	</div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
<style lang="less" scoped>
	.banner{
		height: 500px;
		background: #ccc;
	}
</style>
