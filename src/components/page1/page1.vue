<template>
  <div>
    <!--Navbar here -->
    <mnav
      imgPath="https://res.cloudinary.com/alphajeez/image/upload/v1597615351/user1_vlpp2n.png"
      username="Chioma Davis"
      useremail="Chioma@natterbase"
    ></mnav>

    <!--topnav here -->
    <topnav duration="6 weeks"></topnav>

    <!--Icon here -->
    <icon></icon>

    <div class="container mt-4">
      <div class="row row-cols-5 main ml-5 pl-1">
        <!-- Backlog here -->
        <backlog title="Backlog"></backlog>

        <!-- Todo Columns here -->
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

    <!--Footer here -->
    <mfoot></mfoot>
  </div>
</template>

<script>
  import mnav from "../partials/navbar";
  import topnav from "../partials/topnav";
  import backlog from "../Layout/backlog";
  import todo from "../Layout/todos";
  import mfoot from "../partials/footer";
  import icon from "../Layout/addicon";
  export default {
    name: "page1",
    components: {
      mnav,
      topnav,
      backlog,
      todo,
      mfoot,
      icon,
    },
  };
</script>
