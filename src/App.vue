<template>
  <div id="app">
   <Nav/>
   <Main/>
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
   Nav,
   Main
  }
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  
}
a{
  text-decoration: none;
}
</style>
