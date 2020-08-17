<template>
  <div id="app">
    <sidenav></sidenav>
   <!-- <mnav></mnav> -->
    <router-view />
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Mulish:wght@800&family=Nunito+Sans:wght@300;400;600&display=swap");
:root {
  --background-color: #f7f7f7;
  --muli-font: "Mulish", sans-serif;
  --primary-font-family: "Nunito Sans", sans-serif;
  --main-font-size: 14px;
  --primary-font-10: 10px;
  --primary-font-size: 14px;
  --primary-font-size: 18px;
}
#app {
  font-family: var(--primary-font-family);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background: var(--background-color);
}
</style>

<script>
// import mnav from "./components/partials/navbar";
import sidenav from "./components/partials/sidebar";
export default {
  components: {
    // mnav,
    sidenav,
  },
};
</script>
