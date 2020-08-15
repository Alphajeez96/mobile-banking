<template>
  <div>
    <header>
      <!-- Navbar component here -->
      <section class="container">
        <nav class="navbar navbar-expand-lg navbar-light">
          <span>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="28"
              height="20"
              viewBox="0 0 28 20"
              fill="none"
            >
              <path
                d="M27 0H1C0.734784 0 0.48043 0.105357 0.292893 0.292893C0.105357 0.48043 0 0.734784 0 1C0 1.26522 0.105357 1.51957 0.292893 1.70711C0.48043 1.89464 0.734784 2 1 2H27C27.2652 2 27.5196 1.89464 27.7071 1.70711C27.8946 1.51957 28 1.26522 28 1C28 0.734784 27.8946 0.48043 27.7071 0.292893C27.5196 0.105357 27.2652 0 27 0Z"
                fill="#03293D"
              />
              <path
                d="M1 11H14C14.2652 11 14.5196 10.8946 14.7071 10.7071C14.8946 10.5196 15 10.2652 15 10C15 9.73478 14.8946 9.48043 14.7071 9.29289C14.5196 9.10536 14.2652 9 14 9H1C0.734784 9 0.48043 9.10536 0.292893 9.29289C0.105357 9.48043 0 9.73478 0 10C0 10.2652 0.105357 10.5196 0.292893 10.7071C0.48043 10.8946 0.734784 11 1 11Z"
                fill="#03293D"
              />
              <path
                d="M23 18H1C0.734784 18 0.48043 18.1054 0.292893 18.2929C0.105357 18.4804 0 18.7348 0 19C0 19.2652 0.105357 19.5196 0.292893 19.7071C0.48043 19.8946 0.734784 20 1 20H23C23.2652 20 23.5196 19.8946 23.7071 19.7071C23.8946 19.5196 24 19.2652 24 19C24 18.7348 23.8946 18.4804 23.7071 18.2929C23.5196 18.1054 23.2652 18 23 18Z"
                fill="#03293D"
              />
            </svg>
          </span>
          <!-- Logo here -->
          <a class="navbar-brand a-text mx-5 flex" href="#">
            <img src="../../assets/Logo.png" alt="Logo" />
            <span class="mx-2">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
              >
                <g opacity="0.8">
                  <path
                    d="M13 12C13 11.4477 12.5523 11 12 11C11.4477 11 11 11.4477 11 12C11 12.5523 11.4477 13 12 13C12.5523 13 13 12.5523 13 12Z"
                    stroke="#03293D"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M6 12C6 11.4477 5.55228 11 5 11C4.44772 11 4 11.4477 4 12C4 12.5523 4.44772 13 5 13C5.55228 13 6 12.5523 6 12Z"
                    stroke="#03293D"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M20 12C20 11.4477 19.5523 11 19 11C18.4477 11 18 11.4477 18 12C18 12.5523 18.4477 13 19 13C19.5523 13 20 12.5523 20 12Z"
                    stroke="#03293D"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </g>
              </svg>
            </span>
          </a>
         
         <!-- search bar here -->
         <div class="search__area">
         <span><svg xmlns="http://www.w3.org/2000/svg" width="1" height="30" viewBox="0 0 1 30" fill="none">
<line opacity="0.1" x1="0.5" y1="5.82819e-08" x2="0.499997" y2="30" stroke="#2D2D2D"/>
</svg></span>

 <div class="form-group has-search mx-3">

  <!-- <span
      @mouseover="hover = !hover"
      @mouseleave="hover = !hover"
      :class="{ actives: hover }"
    >
      Hover me to 
    </span> -->

    <span class=" form-control-feedback"></span>
    <input type="text" class="form-control" placeholder="Search">
  </div>

   

  
         </div>

          <!-- <button class="navbar-toggler" style="color: lemonchiffon !important;" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button> -->

          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto"></ul>

            <ul class="navbar-nav my-2 my-lg-0">
              <li class="nav-item active">
                <a class="nav-link mx-3" href="#">About</a>
              </li>
              <li class="nav-item active">
                <a class="nav-link mx-3" href="#">Stories</a>
              </li>
              <li class="nav-item active">
                <a class="nav-link mx-3" href="#">FAQ</a>
              </li>
              <li class="nav-item active">
                <a class="nav-link mx-3" href="#">Blog</a>
              </li>
              <li class="nav-item active">
                <a class="nav-link mx-3" href="#">Login</a>
              </li>
            </ul>
          </div>
        </nav>
      </section>
    </header>
  </div>
</template>
<script>
export default {
    data() {
        return {
             hover: false,
        }
    }
}
</script>
<style scoped>
header {
  width: 100%;
  background: #fbfbfb;
}

.nav-item {
  font-family: 'Poppins', sans-serif;
  color: #000000;
  font-weight: 600;
  font-size: 14px;
  line-height: 19px;
  font-style: normal;
}
.actives {
  background: green;
}
.search__area{
    display:flex;
    	justify-content: center;
}
</style>

