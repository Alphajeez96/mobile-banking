<template>
  <div class="container pl-0 ">
    <div class="d-flex bd-highlight mx-3">
      <!-- top nav here -->
      <div class="flex-fill bd-highlight ">
        <div class="top__nav d-flex">
          <ul class="border-b d-inline-flex" >
            <a href class="active top__nav__link" v-for="tab in tabs " :key="tab"  @click="selected = tab; "  :class="['tab-btn', { active: selected === tab }]">
              <li>{{tab}}</li>
            </a>     
          </ul>
             <component :is="selected" class="tab"></component>
        </div>
      </div>

      <!-- Top nav second division here -->
      <div class="mt-4 flex-fill d-flex bd-highlight">
        <!-- Toggle Switch  here -->
        <p class="mx-3 task">All Task</p>
        <label class="switch ">
          <input type="checkbox" checked />
          <span class="slider round"></span>
        </label>
        <p class="mx-4 modules">All Modules</p>

        <!-- Project deadline  here -->
        <div class="d-flex">
          <span class='mx-2'>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="18"
              height="18"
              viewBox="0 0 18 18"
              fill="none"
            >
              <path
                d="M9 0C4.02934 0 0 4.02955 0 9C0 13.9707 4.02934 18 9 18C13.9707 18 18 13.9707 18 9C18 4.02955 13.9707 0 9 0ZM9 16.3636C4.93323 16.3636 1.63636 13.067 1.63636 9C1.63636 4.93323 4.93323 1.63636 9 1.63636C13.0668 1.63636 16.3636 4.93323 16.3636 9C16.3636 13.067 13.0668 16.3636 9 16.3636ZM12.033 10.8761C12.3525 11.1956 12.3525 11.7137 12.033 12.0332C11.8735 12.1927 11.6638 12.2727 11.4545 12.2727C11.2453 12.2729 11.0358 12.193 10.8761 12.0332L8.42155 9.57866C8.26814 9.42525 8.18182 9.21723 8.18182 9V4.09091C8.18182 3.63907 8.54816 3.27273 9 3.27273C9.45184 3.27273 9.81818 3.63907 9.81818 4.09091V8.66127L12.033 10.8761Z"
                fill="#4DBD98"
              />
              <path
                d="M9 0C4.02934 0 0 4.02955 0 9C0 13.9707 4.02934 18 9 18C13.9707 18 18 13.9707 18 9C18 4.02955 13.9707 0 9 0ZM9 16.3636C4.93323 16.3636 1.63636 13.067 1.63636 9C1.63636 4.93323 4.93323 1.63636 9 1.63636C13.0668 1.63636 16.3636 4.93323 16.3636 9C16.3636 13.067 13.0668 16.3636 9 16.3636ZM12.033 10.8761C12.3525 11.1956 12.3525 11.7137 12.033 12.0332C11.8735 12.1927 11.6638 12.2727 11.4545 12.2727C11.2453 12.2729 11.0358 12.193 10.8761 12.0332L8.42155 9.57866C8.26814 9.42525 8.18182 9.21723 8.18182 9V4.09091C8.18182 3.63907 8.54816 3.27273 9 3.27273C9.45184 3.27273 9.81818 3.63907 9.81818 4.09091V8.66127L12.033 10.8761Z"
                fill="#4DBD98"
              />
              <path
                d="M9 0C4.02934 0 0 4.02955 0 9C0 13.9707 4.02934 18 9 18C13.9707 18 18 13.9707 18 9C18 4.02955 13.9707 0 9 0ZM9 16.3636C4.93323 16.3636 1.63636 13.067 1.63636 9C1.63636 4.93323 4.93323 1.63636 9 1.63636C13.0668 1.63636 16.3636 4.93323 16.3636 9C16.3636 13.067 13.0668 16.3636 9 16.3636ZM12.033 10.8761C12.3525 11.1956 12.3525 11.7137 12.033 12.0332C11.8735 12.1927 11.6638 12.2727 11.4545 12.2727C11.2453 12.2729 11.0358 12.193 10.8761 12.0332L8.42155 9.57866C8.26814 9.42525 8.18182 9.21723 8.18182 9V4.09091C8.18182 3.63907 8.54816 3.27273 9 3.27273C9.45184 3.27273 9.81818 3.63907 9.81818 4.09091V8.66127L12.033 10.8761Z"
                fill="#4DBD98"
              />
              <path
                d="M9 0C4.02934 0 0 4.02955 0 9C0 13.9707 4.02934 18 9 18C13.9707 18 18 13.9707 18 9C18 4.02955 13.9707 0 9 0ZM9 16.3636C4.93323 16.3636 1.63636 13.067 1.63636 9C1.63636 4.93323 4.93323 1.63636 9 1.63636C13.0668 1.63636 16.3636 4.93323 16.3636 9C16.3636 13.067 13.0668 16.3636 9 16.3636ZM12.033 10.8761C12.3525 11.1956 12.3525 11.7137 12.033 12.0332C11.8735 12.1927 11.6638 12.2727 11.4545 12.2727C11.2453 12.2729 11.0358 12.193 10.8761 12.0332L8.42155 9.57866C8.26814 9.42525 8.18182 9.21723 8.18182 9V4.09091C8.18182 3.63907 8.54816 3.27273 9 3.27273C9.45184 3.27273 9.81818 3.63907 9.81818 4.09091V8.66127L12.033 10.8761Z"
                fill="#4DBD98"
              />
            </svg>
          </span>
          <p class="mx-2 deadline">
            Project Dealine :
            <span>{{duration}}</span>
          </p>
        </div>
      </div>
    </div>
  
  </div>
</template>

<script>
import page1 from '../page1/page1'
export default {
  components:{
    page1
  },
  data() {
    return {
       tabs: ["Overview", "Teams", "Modules", "Files", "Progress"],
       selected:'page1',
      duration: "6 weeks",
    };
  },
};
</script>

<style scoped>
.top__nav {
  padding: 15px 70px;
}
ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.border-b {
  border-bottom: 1px solid #797979;
}
.top__nav__link {
  color: #03293d;
  font-weight: bold;
  line-height: 40px;
  padding: 0px 20px;
 font-size: var(--main-font-size);
 opacity: 0.5;
}

.top__nav__link .active {
  border-bottom: 1px solid #f15832;
  opacity: 1;
}
a {
  text-decoration: none !important;
}

/* switch toggle here */

.switch {
  position: relative;
  display: inline-block;
  width: 40px;
  height: 20px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #23B3E8;;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 11px;
  width: 11px;
  left: 1px;
  bottom: 5px;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

input:checked + .slider {
  background-color: #f15832;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
.task{
  color: #23B3E8;
  font-weight: bold;
  font-size: var(--main-font-size);
}
.modules{
 color: #F15832;;
  font-weight: bold;
  font-size: var(--main-font-size);
}
.deadline{
  color:#4DBD98;
  font-size: var(--main-font-size);
  font-weight: bold;
}
</style>