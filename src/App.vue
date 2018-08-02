<template>
  <div id="app">
    <!--<router-view/>-->
    <!--<toast></toast>-->
    <input type="button" value="显示弹窗" @click="showToast"/>
    <hello-world></hello-world>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  methods: {
    showToast () {
      this.$toast('我就是弹窗呀')
    }
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
  margin-top: 60px;
}
</style>
