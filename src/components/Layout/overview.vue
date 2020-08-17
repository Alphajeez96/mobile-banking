<template>
  <div>
    <div class="text-left header">
      <div>{{title}}</div>
    </div>

    <div class="overview__card mt-3">
      <div class="row">
        <div class="c">
          <!--Overview Cards here-->
          <div class="p-3 d-flex flex-wrap">
            <card title="Total Modules" count="20"></card>
            <card title="Improvement" count="20"></card>
            <card title="Total Modules test" count="14"></card>
            <card title="Totail Failed" count="20"></card>
            <card title="Total Passed" count="20"></card>
            <card title="Total Untested" count="20"></card>
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
</script>>

<style scoped>
.header {
  color: #03293d;
  font-size: var(--main-font-size);
  font-weight: Bold;
}
.overview__card {
  background: white;
  padding-bottom: 150px;
  flex-flow: row-reverse wrap;
}
</style>