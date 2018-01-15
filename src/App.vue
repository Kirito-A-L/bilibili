<template>
  <div id="app">
   <one-header/>
    <one-menu/>
    <div class="main">
      <router-view/>
    </div>
  </div>
</template>

<script>
import oneHeader from "./components/header.vue"
import oneMenu from "./components/menu.vue"
export default {
  name: 'App',
  data:function(){
    return {show:true}
  },
  components:{
    oneHeader,
    oneMenu
  },
  methods:{
    
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
