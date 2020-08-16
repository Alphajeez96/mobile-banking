<template>
  <div>
  <topnav></topnav> 
  <backlog></backlog>
  
  </div>
</template>

<script>
import topnav from '../partials/topnav'
import backlog from './backlog'
export default {
  name: 'page1',
  components: {
    topnav,backlog
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
