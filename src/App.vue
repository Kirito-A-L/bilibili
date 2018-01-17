<template>
  <div id="app">
    <OneHeader/>
    <OneMenu/>
    <div class="main">
      <router-view/>
    </div>
  </div>
</template>

<script>
import OneHeader from "@/components/Header.vue"
import OneMenu from "@/components/Menu.vue"
export default {
  name: 'App',
  data:function(){
    return {show:true}
  },
  components:{
    OneHeader,
    OneMenu
   
  },
  methods:{
    toggleMenu:function(){
      this.show = !show;
    }
  }
}
</script>


