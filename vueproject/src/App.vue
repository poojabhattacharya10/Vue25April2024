<template>
  <!-- <MyTest/> -->
  <!-- <MyHome/> -->
  <MyModel/>
</template>

<script>

//  import MyHome from './components/MyHome.vue'
//  import MyTest from './components/MyTest'
import MyModel from './components/MyModel'

export default {
  name: 'App',
  components: {
    // MyTest
    // MyHome
    MyModel
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
