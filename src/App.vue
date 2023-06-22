<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <carousel />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import carousel from './components/carousel.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    carousel
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kablammo&family=Poppins&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
    font-family: 'Poppins';
}.title{font-family: 'Kablammo';color: #ef0a0a;}.texto{color: #ef0a0a;}a{cursor: pointer; text-decoration: none;}br{
    width: 100%;
    border-bottom: 2px solid #ef0a0a;
}
body{
    background-color: #fff;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
