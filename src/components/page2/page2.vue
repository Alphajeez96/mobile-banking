<template>
  <div>

    <topnav></topnav>

    <div class="container mt-4 ">
      <div class="row row-cols-5 main ml-5 pl-1">

      <div class="col-md-3">
         <!-- Backlog here -->
        <backlog title="Modules"></backlog>
      </div>

      <div class="col-md-4">
      qqq
      </div>

         <div class="col-md-4">
      sss
      </div>
     
     
        <!-- Todo Header Column here -->
        
        
      </div>
    </div>
  </div>
</template>

<script>
import mnav from '../partials/navbar'
import topnav from "../partials/topnav2";
import backlog from "../Layout/backlog";
import todo from "../Layout/todos";
export default {
  name: "page1",
  components: {
      mnav,
    topnav,
    backlog,
    todo,
  },
};
</script>
