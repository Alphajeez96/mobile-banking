<template>
  <div>
  <topnav></topnav> 
  <backlog></backlog>
  
  </div>
</template>

<script>
import topnav from '../partials/topnav'
import backlog from '../Layout/backlog'
export default {
  name: 'page1',
  components: {
    topnav,backlog
  }
}
</script>
