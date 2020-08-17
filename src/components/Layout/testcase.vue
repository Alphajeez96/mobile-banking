<template>
    <div>
        <!-- Todo Header Column here -->
    <div >
      <div class="text-left header">
        <div>{{title}}</div> 
      </div>

       <div class="Testcase__cards mt-3">
       
       </div>
    </div>
    </div>
</template>

<script>
export default {
    props: ['title']
}
</script>
<style scoped>
.header {
  color: #03293d;
  font-size: var(--main-font-size);
  font-weight: Bold;
}
.Testcase__cards{
     background: white;
  height: 120vh;
}
</style>>