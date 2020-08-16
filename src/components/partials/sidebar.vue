<template>
  <div>
    <!-- side nav here -->
    <aside class="side__nav position-fixed overflow-auto ">
      <!-- side logo here -->
      <span class="side__logo d-flex align-items-center px-3 py-4">
        <img src="../../assets/General/sidelogo.png" alt />
      </span>
      <div class="border-b mb-4"></div>

      <!--first side nav-items here -->
      <span class="side__nav__items d-flex align-items-center px-3 py-3" v-for="item in items1" :key="item.id">
        <span class="ml-2 flex align-items-center ">
          <img :src="item.icon" alt srcset />
             <!-- <span>Home</span> -->
        </span>
      </span>
      <div class="border-b mb-4"></div>

       <!--Second side nav-items here -->
      <span class="side__nav__items d-flex align-items-center px-3 py-3" v-for="item in items1" :key="item.id">
        <span class="ml-2 flex align-items-center ">
          <img :src="item.icon" alt srcset />
             <!-- <span>Home</span> -->
        </span>
      </span>
      <div class="border-b"></div>
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
    };
  },
};
</script>

<style scoped>
.side__nav {
 
  height: 100%;
  background: #052231;
  width: 80px;
}

.side__logo {
width:100%
}

.border-b {
  border-bottom: 1px solid #e8e7ea;
  opacity: 0.1;
}

.side__nav__items {
  cursor: pointer;
}
</style>