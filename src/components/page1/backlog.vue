<template>
  <div>
    <div class="container mt-4">
      <div class="row row-cols-5 main">
        <div class="col">
        <!-- Header row here -->
          <div class="row header">
            <div class="col">Backlog</div>
            <div class="col">...</div>
          </div>

  <!-- Add log card  here -->
          <div class="add__log__card mt-3 ">
          <span>+</span>
          </div>
        </div>
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.add__log__card{
    background: #FFFFFF;
box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.1);
border-radius: 5px;
height: 30px;
}
</style>