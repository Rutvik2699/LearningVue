<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <Home/> -->
  <Home data="Rutvik is here"  msg="Home is here"/>
  <HomeOne></HomeOne>
  <template-in-vue></template-in-vue>
</template>

<script>
import TemplateInVue from './components/TemplateInVue.vue'
//import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
//import HomeOne from './components/HomeOne.vue'
export default {
  name: 'App',
  components: {
    TemplateInVue
 //   HelloWorld,
    // Home,

    //Home one is component to learn the nesting of the components
    //It is connected to MyUsers,ProductsSi and HomeOne
    //HomeOne


  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
