<template>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
@Component({
    components: {
      
    },
    methods:{
      btnClick:function(e){
        console.log('btnClicked...');  
      }
    }
  })
export default class AppNav extends Vue {}
</script>
<style scoped lang="scss">
#nav {
  padding: 10px;
  border: 1px solid blue;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>