<template>
  <div>
    <!-- Testcase Header Column here -->
    <div>
      <div class="text-left header">
        <div>{{ title }}</div>
      </div>

      <div class="Testcase__cards text-left mt-3">
        <div class="d-flex bd-highlight mb-2" v-for="i in 8" :key="i">
          <!-- Testcase card text-->
          <div class="mr-auto pt-3 px-3">
            <p>Make the Background Image blur</p>
          </div>

          <!-- custom select-->
          <div class="pt-3 px-3">
            <v-select class="style-chooser" :options="options"></v-select>
          </div>
        </div>

        <!--Test case buttons here-->
        <div class="d-flex bd-highlight">
          <div class="mr-auto mt-3 mb-5 px-3">
            <button class="new__test__btn">New Test Case</button>
          </div>
          <div class="mb-5 mt-3 px-3">
            <button class="test__btn">Test</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    props: ["title"],
    data() {
      return {
        options: ["Pass", "Failed", "Retest", "Untest"],

        open: false,
      };
    },
    mounted() {
      this.$emit("input", this.selected);
    },
  };
</script>
<style scoped>
  .header {
    color: #03293d;
    font-size: var(--main-font-size);
    font-weight: Bold;
  }
  .Testcase__cards {
    background: white;
  }
  .Testcase__cards p {
    color: #03293d;
    font-weight: bold;
    font-size: 14px;
  }
  .new__test__btn {
    background: #23b3e8;
    border: 2px solid rgba(26, 12, 47, 0.1);
    border-radius: 5px;
    color: white;
    font-weight: bold;
    font-size: 14px;
    padding: 5px 15px;
  }
  .test__btn {
    background: #ffffff;
    border: 2px solid #03293d;
    border-radius: 5px;
    color: #03293d;
    font-weight: bold;
    font-size: 14px;
    padding: 5px 40px;
  }
  .new__test__btn:focus,
  .test__btn:focus {
    outline: 0;
  }
</style>
