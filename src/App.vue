<template>
  <div class="container">
    <Sidebar />
    <Main />
  </div> 
</template>

<script>
import Sidebar from './components/sidebar.vue'
import Main from './components/main.vue'

export default {
  name: 'App',
  components: {
    Sidebar,
    Main
  }
}
</script>

<style>
html, body { 
  width:100%;
  height:100%;
  padding:0;
  margin:0;
}
#app {
  height:100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.container {
  display:flex;
  width:100%;
  height:100%;
}
</style>
