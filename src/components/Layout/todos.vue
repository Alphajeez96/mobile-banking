<template>
  <div>
    <!-- Todo Header Column here -->
    <div class="col">
      <div class="row header">
        <div>{{ title }}</div>
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

    <!-- Todo card place hoders here  here -->
    <div class="placeholder__cards mt-3"></div>
  </div>
</template>

<script>
  export default {
    name: "todos",
    props: ["title"],
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
  .placeholder__cards {
    background: linear-gradient(
      180deg,
      #ffffff 0%,
      rgba(255, 255, 255, 0) 100%
    );
    height: 120vh;
  }
  .header {
    color: #03293d;
    font-size: var(--main-font-size);
    font-weight: Bold;
  }
  .dots {
    position: relative;
    left: 40px;
  }
</style>
