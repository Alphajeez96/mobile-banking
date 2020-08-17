<template>
  <div>
 <mnav imgPath='https://res.cloudinary.com/alphajeez/image/upload/v1597615351/user1_vlpp2n.png' username='Chioma Davis' useremail='Chioma@natterbase'></mnav>
    <topnav duration='6 weeks'></topnav>

    <div class="container mt-4 ">
      <div class="row row-cols-5 main ml-5 pl-1">
        <!-- Backlog here -->
        <backlog title="Backlog"></backlog>

        <!-- Todo Header Column here -->
        <div class="col">
          <todo title="Todo"></todo>
        </div>

        <div class="col">
          <todo title="In Progress"></todo>
        </div>

        <div class="col">
          <todo title="In Review"></todo>
        </div>

        <div class="col">
          <todo title="Done"></todo>
        </div>
        
      </div>
    </div>
    <mfoot></mfoot>
  </div>
</template>

<script>
import mnav from '../partials/navbar'
import topnav from "../partials/topnav";
import backlog from "../Layout/backlog";
import todo from "../Layout/todos";
import mfoot from '../partials/footer'
export default {
  name: "page1",
  components: {
    mnav,
    topnav,
    backlog,
    todo,
    mfoot
  },
  data(){
    return {
      url: 'https://res.cloudinary.com/alphajeez/image/upload/v1597615351/user1_vlpp2n.png'
    }
  }
  
};
</script>
