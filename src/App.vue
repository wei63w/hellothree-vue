<template>
  <div id="app">
    <AppNav></AppNav>
    <router-view/>
  </div>
</template>



<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
import AppNav from '@/components/AppNav.vue'
 
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

import $ from 'jquery'

@Component({
    components: {
      AppNav
    },
    methods:{
      btnClick:function(e){
        console.log('btnClicked...');  
      }
    }
  })
export default class App extends Vue {}
</script>


<style lang="scss">


#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
