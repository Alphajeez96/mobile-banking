<template>
    <div>
 <div>
  <div class="cards mx-2 mt-4">
   
  </div>
</div>
    </div>
</template>

<script>
export default {
    name: 'card',
    props:['title','backgroundColor' ]
}
</script>
<style scoped>
.cards{
  width: 160px;
height: 112px;
box-shadow: 0px 0px 2px rgba(0, 0, 0, 0.15);
border-radius: 5px;
}
</style>