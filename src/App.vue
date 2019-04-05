<template>
  <div id="app">
    
    <HelloWorld />
    <SlideShow />
    <ZhuTi />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SlideShow from  './components/SlideShow.vue'
import ZhuTi from './components/ZhuTi.vue'
export default {
  name: 'app',
  components: {
    HelloWorld,
    SlideShow,
    ZhuTi
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
