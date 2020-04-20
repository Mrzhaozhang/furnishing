<template>
  <div id="app">
	<top-menu></top-menu>
    <router-view/>
  </div>
</template>
<script>
	import TopMenu from './components/Topmenu.vue'
	export default{
		components:{
			TopMenu
		}
	}
</script>
<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
