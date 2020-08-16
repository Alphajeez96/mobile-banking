<template>
  <div>
    <!-- side nav here -->
    <aside class="side__nav position-fixed overflow-auto">
    
      <!-- side logo here -->
      <span class="side__logo d-flex align-items-center px-3 py-4">
        <img src="../../assets/General/sidelogo.png" alt />
      </span>
      <div class="border-b mb-4"></div>

      <!--first side nav-items here -->
      <span
        class="side__nav__items d-flex align-items-center px-3 py-3"
        v-for="item in items1"
        :key="item.id"
      >
        <span class="ml-2 flex align-items-center">
          <img :src="item.icon" alt srcset />
          <!-- <span>Home</span> -->
        </span>
      </span>
      <div class="border-b mb-4"></div>

      <!--Second side nav-items here -->
      <span
        class="side__nav__items d-flex align-items-center px-3 py-3"
        v-for="item in items2"
        :key="item.id"
      >
        <span class="ml-2 flex align-items-center">
          <img :src="item.icon" alt srcset />
          <!-- <span>Home</span> -->
        </span>
      </span>
      <div class="border-b mb-4"></div>

      <!--Logout nav-items here -->
      <span class="side__nav__items logout d-flex align-items-center px-3 py-3">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="40"
          height="40"
          viewBox="0 0 40 40"
          fill="none"
        >
          <rect opacity="0.2" width="40" height="40" rx="20" fill="#E8E7EA" />
          <path
            d="M18 25L23 20L18 15"
            stroke="#23B3E8"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </span>
    </aside>
  </div>
</template>


<script>
export default {
  data() {
    return {
      drawer: false,

      items1: [
        {
          text: "Home",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='17' height='19' viewBox='0 0 17 19' fill='none'%3E%3Cpath d='M6 17.6667V9.33333H11V17.6667M1 6.83333L8.5 1L16 6.83333V16C16 16.442 15.8244 16.866 15.5118 17.1785C15.1993 17.4911 14.7754 17.6667 14.3333 17.6667H2.66667C2.22464 17.6667 1.80072 17.4911 1.48816 17.1785C1.17559 16.866 1 16.442 1 16V6.83333Z' stroke='white' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E",
          route: "/",
        },
        {
          text: "Returns",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='15' height='15' viewBox='0 0 15 15' fill='none'%3E%3Cpath d='M11.2778 9.22222C10.1425 9.22222 9.22222 10.1425 9.22222 11.2778C9.22222 12.413 10.1425 13.3333 11.2778 13.3333C12.413 13.3333 13.3333 12.413 13.3333 11.2778C13.3333 10.1425 12.413 9.22222 11.2778 9.22222ZM11.2778 9.22222V4.42593C11.2778 4.06248 11.1334 3.71392 10.8764 3.45693C10.6194 3.19993 10.2709 3.05556 9.90741 3.05556H7.85185M3.05556 5.11111C4.19081 5.11111 5.11111 4.19081 5.11111 3.05556C5.11111 1.9203 4.19081 1 3.05556 1C1.9203 1 1 1.9203 1 3.05556C1 4.19081 1.9203 5.11111 3.05556 5.11111ZM3.05556 5.11111V13.3333' stroke='%23FCFCFC' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E",
          route: "/returns",
        },
        {
          text: "Users",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='19' height='15' viewBox='0 0 19 15' fill='none'%3E%3Cpath d='M13.0964 13.9111V12.5037C13.0964 11.7572 12.7999 11.0412 12.272 10.5133C11.7441 9.98545 11.0281 9.68889 10.2816 9.68889H4.65197C3.90544 9.68889 3.18948 9.98545 2.6616 10.5133C2.13372 11.0412 1.83716 11.7572 1.83716 12.5037V13.9111M17.3186 13.9111V12.5037C17.3182 11.88 17.1106 11.2742 16.7285 10.7813C16.3464 10.2883 15.8114 9.93629 15.2075 9.78037M12.3927 1.33593C12.9982 1.49095 13.5349 1.84309 13.9181 2.33681C14.3013 2.83054 14.5093 3.43777 14.5093 4.06278C14.5093 4.68779 14.3013 5.29502 13.9181 5.78874C13.5349 6.28247 12.9982 6.6346 12.3927 6.78963M10.2816 4.05926C10.2816 5.61384 9.02137 6.87408 7.46679 6.87408C5.91221 6.87408 4.65197 5.61384 4.65197 4.05926C4.65197 2.50468 5.91221 1.24445 7.46679 1.24445C9.02137 1.24445 10.2816 2.50468 10.2816 4.05926Z' stroke='%23FCFCFC' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E",
          route: "/users",
        },
        {
          text: "Folder",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='13' viewBox='0 0 16 13' fill='none'%3E%3Cpath d='M13.8664 3.03714V1.65207L4.53286 1.65174V3.03681L13.8664 3.03714ZM13.8665 8.57707L13.8663 5.11494L4.53277 5.1146L4.53302 8.57673L13.8665 8.57707ZM13.8664 0.267002C14.6031 0.267002 15.1998 0.886102 15.1998 1.65207L15.1999 8.57707C15.1999 9.34309 14.6033 9.96214 13.8665 9.96214L4.53302 9.9618C3.79631 9.9618 3.19963 9.34274 3.19963 8.57673L3.20614 1.65174C3.20614 0.885762 3.79614 0.266663 4.53286 0.266663L13.8664 0.267002ZM1.86665 11.3483H11.8671V12.7333L1.86681 12.733C1.1301 12.733 0.533424 12.1139 0.533424 11.3479L0.533264 3.73036H1.86665V11.3483Z' fill='white'/%3E%3C/svg%3E",
          route: "/folder",
        },
      ],

      items2: [
        {
          text: "PN",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16' fill='none'%3E%3Crect width='16' height='16' rx='8' fill='%2323B3E8'/%3E%3Cpath d='M4.456 5.77H6.304C6.756 5.77 7.108 5.884 7.36 6.112C7.612 6.336 7.738 6.652 7.738 7.06C7.738 7.468 7.612 7.786 7.36 8.014C7.108 8.242 6.756 8.356 6.304 8.356H5.23V10H4.456V5.77ZM6.208 7.762C6.74 7.762 7.006 7.53 7.006 7.066C7.006 6.83 6.94 6.656 6.808 6.544C6.676 6.428 6.476 6.37 6.208 6.37H5.23V7.762H6.208ZM11.9869 5.77V10H11.4049L9.13694 7.048V10H8.41694V5.77H8.99294L11.2609 8.716V5.77H11.9869Z' fill='white'/%3E%3C/svg%3E",
          route: "/PN",
        },
        {
          text: "JI",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16' fill='none'%3E%3Crect width='16' height='16' rx='8' fill='%234DBD98'/%3E%3Crect width='16' height='16' rx='8' fill='%234DBD98'/%3E%3Crect width='16' height='16' rx='8' fill='%234DBD98'/%3E%3Crect width='16' height='16' rx='8' fill='%234DBD98'/%3E%3Cpath d='M5.964 9.43L6.384 9.4C6.74 9.376 6.918 9.18 6.918 8.812V5.77H7.692V8.806C7.692 9.182 7.592 9.474 7.392 9.682C7.196 9.886 6.902 10 6.51 10.024L6.018 10.054L5.964 9.43ZM8.60639 5.77H9.38039V10H8.60639V5.77Z' fill='white'/%3E%3C/svg%3E",
          route: "/JI",
        },
        {
          text: "LG",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16' fill='none'%3E%3Crect width='16' height='16' rx='8' fill='%233D43A2'/%3E%3Cpath d='M4.456 5.77H5.23V9.364H7.204V10H4.456V5.77ZM11.0836 7.714V9.742C10.8916 9.838 10.6576 9.914 10.3816 9.97C10.1096 10.026 9.83161 10.054 9.54761 10.054C9.11161 10.054 8.73361 9.968 8.41361 9.796C8.09361 9.62 7.84761 9.37 7.67561 9.046C7.50761 8.718 7.42361 8.33 7.42361 7.882C7.42361 7.438 7.50761 7.054 7.67561 6.73C7.84761 6.402 8.08961 6.152 8.40161 5.98C8.71761 5.804 9.08761 5.716 9.51161 5.716C9.80761 5.716 10.0856 5.76 10.3456 5.848C10.6056 5.932 10.8216 6.054 10.9936 6.214L10.7356 6.772C10.5396 6.62 10.3456 6.512 10.1536 6.448C9.96561 6.38 9.75761 6.346 9.52961 6.346C9.09361 6.346 8.76361 6.476 8.53961 6.736C8.31961 6.992 8.20961 7.374 8.20961 7.882C8.20961 8.922 8.66561 9.442 9.57761 9.442C9.84961 9.442 10.1216 9.404 10.3936 9.328V8.266H9.48161V7.714H11.0836Z' fill='white'/%3E%3C/svg%3E",
          route: "/LG",
        },
        {
          text: "AW",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16' fill='none'%3E%3Crect width='16' height='16' rx='8' fill='%23F15832'/%3E%3Cpath d='M6.264 9.01H4.206L3.78 10H3L4.914 5.77H5.544L7.458 10H6.69L6.264 9.01ZM6.006 8.41L5.232 6.61L4.458 8.41H6.006ZM13.5648 5.77L12.0708 10H11.4408L10.3788 6.958L9.31083 10H8.68083L7.19283 5.77H7.97283L9.02283 8.92L10.1268 5.77H10.6728L11.7468 8.938L12.8268 5.77H13.5648Z' fill='white'/%3E%3C/svg%3E",
          route: "/AW1",
        },
        {
          text: "AW",
          icon:
            "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 16 16' fill='none'%3E%3Crect width='16' height='16' rx='8' fill='%23004F71'/%3E%3Cpath d='M6.264 9.01H4.206L3.78 10H3L4.914 5.77H5.544L7.458 10H6.69L6.264 9.01ZM6.006 8.41L5.232 6.61L4.458 8.41H6.006ZM13.5648 5.77L12.0708 10H11.4408L10.3788 6.958L9.31083 10H8.68083L7.19283 5.77H7.97283L9.02283 8.92L10.1268 5.77H10.6728L11.7468 8.938L12.8268 5.77H13.5648Z' fill='white'/%3E%3C/svg%3E",
          route: "/AW2",
        },
      ],
    };
  },
};
</script>

<style scoped>
.side__nav {
  height: 100%;
  background: #052231;
  width: 95px;
}

.side__logo {
  width: 100%;
}

.border-b {
  border-bottom: 1px solid #e8e7ea;
  opacity: 0.1;
}

.side__nav__items {
  cursor: pointer;
}
.logout {
  margin-top: 100px;
}

/* Scroll bar here */
::-webkit-scrollbar {
  width: 5px;
}

::-webkit-scrollbar-track {
  background: #052231; 
}
 
::-webkit-scrollbar-thumb {
  background: #888; 
}

::-webkit-scrollbar-thumb:hover {
  background: #555; 
}
</style>