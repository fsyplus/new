<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div>数据{{ name }}</div>
    <button class="haha" @click="back"></button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import router from '@/router';

export default {
  name: 'HomeView',
  components: { 
    HelloWorld 
  },
  data(){
    return {
      name:'送达'
    }
  },
  methods:{
    back(){
      console.log('上班第一天');
    }
  }
}
</script>
<style>
.haha{
  width: 200px;
  height: 200px;
  background-color: red;
}
</style>