<template>
  <div>
  <mnav imgPath='https://res.cloudinary.com/alphajeez/image/upload/v1597615517/user2_cnkbzf.png' username='Mark Dawn' useremail='Markdawn@natterbase'></mnav>

    <topnav duration='6 weeks'></topnav>

    <div class="container   mt-4 ">
      <div class="row row-cols-3">

      <div class="col-md-3">

         <!-- Backlog here -->
        <backlog title="Modules"></backlog>
      </div>

      <div class="col-5">
    <testcases title="Added Test Case"></testcases>
      </div>

         <div class=" ">
    <overview title="Quick Overview"></overview>
      </div>
     
     
        <!-- Todo Header Column here -->
           
      </div>
    </div>
  </div>
</template>

<script>
import mnav from '../partials/navbar'
import topnav from "../partials/topnav";
import backlog from "../Layout/backlog";
import todo from "../Layout/todos";
import testcases from '../Layout/testcase';
import overview from '../Layout/overview'

export default {
  name: "page1",
  components: {
      mnav,
    topnav,
    backlog,
    todo,
    testcases,
    overview
    
  },
};
</script>

<style scoped>
.container{
  padding-left: 70px;
}
</style>>