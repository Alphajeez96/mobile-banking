<template>
  <div>
    <topnav></topnav>

    <div class="container mt-4 ">
      <div class="row row-cols-5 main ml-5 pl-1">
        <!-- Backlog here -->
        <backlog></backlog>

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
  </div>
</template>

<script>
import topnav from "../partials/topnav2";
import backlog from "../Layout/backlog";
import todo from "../Layout/todos";
export default {
  name: "page1",
  components: {
    topnav,
    backlog,
    todo,
  },
};
</script>
