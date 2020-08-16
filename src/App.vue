<template>
  <div id="app">
   <sidenav></sidenav>
  <mnav></mnav>
 
    <router-view/>
  </div>
</template>

<style>
:root{

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #F7F7F7;
}


</style>

<script>
import mnav from './components/partials/navbar'
import sidenav from './components/partials/sidebar'
export default {
  components:{
    mnav, sidenav
  }
}
</script>
