<template>
  <div>
    <!-- Backlog Header COumn here -->
    <div class="col">
      <div class="row header">
        <div class="col-2">{{title}}</div>
        <div class="col dots">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="12"
            height="3"
            viewBox="0 0 12 3"
            fill="none"
          >
            <path
              d="M6.625 1.625C6.625 1.27982 6.34518 1 6 1C5.65482 1 5.375 1.27982 5.375 1.625C5.375 1.97018 5.65482 2.25 6 2.25C6.34518 2.25 6.625 1.97018 6.625 1.625Z"
              fill="#03293D"
              stroke="#03293D"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M2.25 1.625C2.25 1.27982 1.97018 1 1.625 1C1.27982 1 1 1.27982 1 1.625C1 1.97018 1.27982 2.25 1.625 2.25C1.97018 2.25 2.25 1.97018 2.25 1.625Z"
              fill="#03293D"
              stroke="#03293D"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M11 1.625C11 1.27982 10.7202 1 10.375 1C10.0298 1 9.75 1.27982 9.75 1.625C9.75 1.97018 10.0298 2.25 10.375 2.25C10.7202 2.25 11 1.97018 11 1.625Z"
              fill="#03293D"
              stroke="#03293D"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </div>
      </div>

      <!-- Add log card  here -->
      <div class="add__log__card mt-3">
        <span>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="9"
            height="9"
            viewBox="0 0 9 9"
            fill="none"
          >
            <path
              d="M9 5.14286H5.14286V9H3.85714V5.14286H0V3.85714H3.85714V0H5.14286V3.85714H9V5.14286Z"
              fill="#23B3E8"
            />
          </svg>
        </span>
      </div>

      <!-- Back log display card  here -->
      <div class="backlog__card mt-3" v-for="i in 7" :key="i">
        <!-- Text row card  here -->
        <div class="row">
          <div class="col-9 pt-2 text">
            <p>Apply gredient colours on the dashboard sidenav</p>
          </div>
          <div class="col">
            <p>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="12"
                height="3"
                viewBox="0 0 12 3"
                fill="none"
              >
                <path
                  d="M6.625 1.625C6.625 1.27982 6.34518 1 6 1C5.65482 1 5.375 1.27982 5.375 1.625C5.375 1.97018 5.65482 2.25 6 2.25C6.34518 2.25 6.625 1.97018 6.625 1.625Z"
                  fill="#03293D"
                  stroke="#03293D"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M2.25 1.625C2.25 1.27982 1.97018 1 1.625 1C1.27982 1 1 1.27982 1 1.625C1 1.97018 1.27982 2.25 1.625 2.25C1.97018 2.25 2.25 1.97018 2.25 1.625Z"
                  fill="#03293D"
                  stroke="#03293D"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M11 1.625C11 1.27982 10.7202 1 10.375 1C10.0298 1 9.75 1.27982 9.75 1.625C9.75 1.97018 10.0298 2.25 10.375 2.25C10.7202 2.25 11 1.97018 11 1.625Z"
                  fill="#03293D"
                  stroke="#03293D"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </p>
          </div>
        </div>

        <!-- Timeline row card  here -->
        <div class="row">
          <div class="col-8 text">
            <p>
              <span>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="11"
                  height="11"
                  viewBox="0 0 11 11"
                  fill="none"
                >
                  <path
                    d="M5.49983 0.458336C2.71534 0.458336 0.45816 2.71563 0.45816 5.5C0.45816 8.28449 2.71534 10.5417 5.49983 10.5417C8.28432 10.5417 10.5415 8.28449 10.5415 5.5C10.5415 2.71563 8.28432 0.458336 5.49983 0.458336ZM5.49983 9.625C3.22168 9.625 1.37483 7.77826 1.37483 5.5C1.37483 3.22186 3.22168 1.375 5.49983 1.375C7.77797 1.375 9.62483 3.22186 9.62483 5.5C9.62483 7.77826 7.77797 9.625 5.49983 9.625ZM7.19887 6.55096C7.37785 6.72994 7.37785 7.02018 7.19887 7.19916C7.10949 7.28853 6.99205 7.33334 6.87483 7.33334C6.75761 7.33345 6.64028 7.28865 6.55079 7.19916L5.17579 5.82416C5.08985 5.73822 5.04149 5.62169 5.04149 5.5V2.75C5.04149 2.49689 5.24671 2.29167 5.49983 2.29167C5.75294 2.29167 5.95816 2.49689 5.95816 2.75V5.31025L7.19887 6.55096Z"
                    fill="#03293D"
                  />
                </svg>
              </span>
              <span class="mx-2">Due {{date}}</span>
            </p>
          </div>
          <!-- User Images here  here -->
          <div class="col">
            <div class="row img__holder">
              <img class src="../../assets/Vectors/e1.png" alt />
              <img class="position-absolute img__two" src="../../assets/Vectors/e2.png" alt />
              <img class="position-absolute img__three" src="../../assets/Vectors/e3.png" alt />
              <img class="position-absolute img__four" src="../../assets/Vectors/e4.png" alt />
              <div class="position-absolute elipse">
                <span>+4</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "backlog",
    props: ["title"],
  data() {
    return {
      date: "Aug 8",
    };
  },
};
</script>


<style scoped>
.add__log__card {
  background: #ffffff;
  box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
  height: 30px;
  cursor: pointer;
}
.header {
  color: #03293d;
  font-size: var(--main-font-size);
  font-weight: Bold;
}
.backlog__card {
  background: #ffffff;
  border-radius: 5px;
  cursor: pointer;
}
.text p {
  text-align: left;
  font-size: 10px;
  padding: 0px 8px;
  color: #03293d;
}
.img__holder {
  position: relative;
}
.absolute {
  top: 0;
}
.img__two {
  right: 52px;
}
.img__three {
  right: 40px;
}
.img__four {
  right: 30px;
}
.elipse {
  background: #e8e7ea;
  opacity: 0.4;
  height: 15px;
  width: 15px;
  border-radius: 50%;
  right: 20px;
  font-size: 10px;
  color: #a5a4a4;
}
.dots{
  position: relative;
  left: 60px;
}
</style>