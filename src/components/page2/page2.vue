<template>
  <div>

    <topnav></topnav>

    <div class="container mt-4 ">
      <div class="row row-cols-5 main ml-5 pl-1">

      <div class="col-md-3">

         <!-- Backlog here -->
        <backlog title="Modules"></backlog>
      </div>

      <div class="col-md-5">
    <testcases title="Added Test Case"></testcases>
      </div>

         <div class="col-md-4">
    <overview title="Quick Overview"></overview>
      </div>
     
     
        <!-- Todo Header Column here -->
           
      </div>
    </div>
  </div>
</template>

<script>

import topnav from "../partials/topnav2";
import backlog from "../Layout/backlog";
import todo from "../Layout/todos";
import testcases from '../Layout/testcase';
import overview from '../Layout/overview'

export default {
  name: "page1",
  components: {
      
    topnav,
    backlog,
    todo,
    testcases,
    overview
    
  },
};
</script>
