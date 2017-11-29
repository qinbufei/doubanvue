<template>  
  <div id="div">
    <img src="./assets/logo.png" alt="">
    <h1>{{msg}}</h1>
    <ul>
      <li><router-link to="/first">点我跳第一条</router-link></li>
      <li><router-link to="/second">点我跳第二条</router-link></li>
    </ul>
    <router-view class="view"></router-view>
  </div>
</template> 

<script>
import firstcomponent from './component/firstcomponent.vue'
import secondcomponent from './component/secondcomponent.vue'
export default {
  data(){
    return {
      msg:'hello vue',
    }
  },
  components:{firstcomponent,secondcomponent},
}
</script>

<style>
  body{
    font-family: Arial, Helvetica, sans-serif;
  }
</style>

