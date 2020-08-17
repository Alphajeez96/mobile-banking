<template>
  <div>
    <div class="text-left header">
      <div>{{ title }}</div>
    </div>
    <div class="overview__card mt-3">
      <div class="row">
        <div>
          <!-- Overview Cards passed down as props here-->
          <div class="p-3 d-flex flex-wrap">
            <card title="Total Modules" count="20" color="#F15832;"></card>
            <card
              title="Improvement"
              count="20"
              color="rgba(3, 41, 61, 0.8);"
            ></card>
            <card
              title="Total Modules test"
              count="14"
              color=" #296799;"
            ></card>
            <card title="Totail Failed" count="20" color="#F8426E;"></card>
            <card title="Total Passed" count="20" color="#4DBD98;"></card>
            <card title="Total Untested" count="20" color="#3D43A2;"></card>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  import card from "./card";
  export default {
    components: {
      card,
    },
    props: ["title"],
  };
</script>

<style scoped>
  .header {
    color: #03293d;
    font-size: var(--main-font-size);
    font-weight: Bold;
  }
  .overview__card {
    background: white;
    padding-bottom: 125px;
    flex-flow: row-reverse wrap;
  }
</style>
