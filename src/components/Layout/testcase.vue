<template>
    <div>
        <!-- Todo Header Column here -->
    <div >
      <div class="text-left header">
        <div>{{title}}</div> 
      </div>

       <div class="Testcase__cards text-left mt-3">
       
       <div class="row" v-for="i in 8" :key="i">
       <div class="col-8">
       <p>Make the Background Image blur</p>
       </div>

        <div class="col-4 button__holder">
       hhh
       </div>
       </div>
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
 

}
.Testcase__cards p {
    color: #03293D;
    font-weight: bold;
    font-size: 14px;
 padding: 10px;
    border-left: 1px solid red
}
.button__holder{
       padding: 10px
}
</style>>