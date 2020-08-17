<template>
  <div class="custom-select" :tabindex="tabindex" @blur="open = false">
    <v-select    class="style-chooser" :options="options"></v-select>
  </div>
</template>

<script>
export default {
  name:'customSelect',

  data() {
    return {
    options: [
      'foo',
      'bar',
      'baz'
    ]
    };
  },
 

};
</script>

<style scoped>
.vs__dropdown-toggle {
   display: none;
}

</style>