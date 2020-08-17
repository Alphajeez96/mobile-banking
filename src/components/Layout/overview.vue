<template>
    <div>
      <div class="text-left header">
        <div>{{title}}</div> 
      </div>

      <div class="overview__card mt-3">
      
      </div>
    </div>
</template>
<script>
export default {
    props: ['title']
}
</script>>

<style scoped>
.header {
  color: #03293d;
  font-size: var(--main-font-size);
  font-weight: Bold;
}
.overview__card{
     background: white;
height: 100vh;
}
</style>>