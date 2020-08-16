<template>
  <div>
    <header>
      <!-- Navbar component here -->
      <section class="container">
        <nav class="navbar navbar-expand-lg navbar-light">
          <!-- Toggler here -->

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
            <img src="../../assets/General/Logo.png" alt="Logo" />
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

          <!-- search area here -->

          <div class="search__area">
            <span>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="1"
                height="30"
                viewBox="0 0 1 30"
                fill="none"
              >
                <line
                  opacity="0.1"
                  x1="0.5"
                  y1="5.82819e-08"
                  x2="0.499997"
                  y2="30"
                  stroke="#2D2D2D"
                />
              </svg>
            </span>

            <!-- search bar -->

            <div class="input-group mx-2">
              <span class="input-group-append">
                <div class="input-group-text bg-inherit">
                  <i class>
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="20"
                      height="20"
                      viewBox="0 0 20 20"
                      fill="none"
                    >
                      <g opacity="0.5">
                        <path
                          d="M9.16667 15.8333C12.8486 15.8333 15.8333 12.8486 15.8333 9.16667C15.8333 5.48477 12.8486 2.5 9.16667 2.5C5.48477 2.5 2.5 5.48477 2.5 9.16667C2.5 12.8486 5.48477 15.8333 9.16667 15.8333Z"
                          stroke="#2D2D2D"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        />
                        <path
                          d="M17.5 17.5L13.875 13.875"
                          stroke="#2D2D2D"
                          stroke-width="2"
                          stroke-linecap="round"
                          stroke-linejoin="round"
                        />
                      </g>
                    </svg>
                  </i>
                </div>
              </span>
              <input
                class="form-control"
                type="search"
                id="example-search-input"
                placeholder="Search"
              />
            </div>
            <!-- <span
      @mouseover="hover = !hover"
      @mouseleave="hover = !hover"
      :class="{ actives: hover }"
    >
      Hover me to 
            </span>-->
          </div>

          <!-- <button class="navbar-toggler" style="color: lemonchiffon !important;" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
          </button>-->

          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto"></ul>

            <!-- Notification panel here -->

            <ul class="navbar-nav my-2 my-lg-0">
              <!-- Notification Icon  -->
              <li class="mx-3">
                <span>
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="none"
                  >
                    <path
                      d="M18 8C18 6.4087 17.3679 4.88258 16.2426 3.75736C15.1174 2.63214 13.5913 2 12 2C10.4087 2 8.88258 2.63214 7.75736 3.75736C6.63214 4.88258 6 6.4087 6 8C6 15 3 17 3 17H21C21 17 18 15 18 8Z"
                      stroke="#2D2D2D"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                    <path
                      d="M13.73 21C13.5542 21.3031 13.3018 21.5547 12.9982 21.7295C12.6946 21.9044 12.3504 21.9965 12 21.9965C11.6496 21.9965 11.3054 21.9044 11.0018 21.7295C10.6982 21.5547 10.4458 21.3031 10.27 21"
                      stroke="#2D2D2D"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </span>
              </li>

             <!-- Owner badge -->
              <li class="mx-3">
                <button type="button" class="owner__btn">
                  <span class="badge">
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="61"
                      height="13"
                      viewBox="0 0 61 13"
                      fill="none"
                    >
                      <path
                        d="M6.49999 11.9167C6.49999 11.9167 10.8333 9.75001 10.8333 6.50001V2.70834L6.49999 1.08334L2.16666 2.70834V6.50001C2.16666 9.75001 6.49999 11.9167 6.49999 11.9167Z"
                        stroke="#FCFCFC"
                        stroke-width="1.5"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                      <path
                        d="M24.98 10.09C24.2733 10.09 23.6567 9.94333 23.13 9.65C22.61 9.35 22.2067 8.92333 21.92 8.37C21.64 7.81667 21.5 7.17 21.5 6.43C21.5 5.69 21.64 5.04667 21.92 4.5C22.2067 3.95333 22.61 3.53333 23.13 3.24C23.6567 2.94 24.2733 2.79 24.98 2.79C25.6867 2.79 26.3 2.94 26.82 3.24C27.34 3.53333 27.74 3.95333 28.02 4.5C28.3 5.04667 28.44 5.69 28.44 6.43C28.44 7.17 28.3 7.81667 28.02 8.37C27.74 8.92333 27.34 9.35 26.82 9.65C26.3 9.94333 25.6867 10.09 24.98 10.09ZM24.98 8.87C25.58 8.87 26.0467 8.66 26.38 8.24C26.72 7.82 26.89 7.21667 26.89 6.43C26.89 5.64333 26.72 5.04333 26.38 4.63C26.0467 4.21667 25.58 4.01 24.98 4.01C24.38 4.01 23.91 4.21667 23.57 4.63C23.2367 5.04333 23.07 5.64333 23.07 6.43C23.07 7.22333 23.2367 7.83 23.57 8.25C23.91 8.66333 24.38 8.87 24.98 8.87ZM39.8239 2.88L37.2939 10H36.0439L34.3839 5.29L32.7139 10H31.4639L28.9339 2.88H30.5239L32.1639 7.8L33.8839 2.88H34.9739L36.6539 7.87L38.3339 2.88H39.8239ZM46.8937 2.88V10H45.7337L42.1837 5.46V10H40.7237V2.88H41.8737L45.4237 7.41V2.88H46.8937ZM48.3213 2.88H53.2313V4.09H49.8413V5.77H53.0213V6.99H49.8413V8.79H53.2313V10H48.3213V2.88ZM60.3177 10H58.6677L57.7577 7.63C57.6843 7.44333 57.571 7.31333 57.4177 7.24C57.271 7.16667 57.0843 7.13 56.8577 7.13H55.8477V10H54.3077V2.88H57.4777C58.3043 2.88 58.931 3.06 59.3577 3.42C59.7843 3.78 59.9977 4.29667 59.9977 4.97C59.9977 5.44333 59.871 5.85 59.6177 6.19C59.371 6.53 59.0143 6.77333 58.5477 6.92C58.9677 7.00667 59.271 7.29667 59.4577 7.79L60.3177 10ZM57.2477 5.94C57.6943 5.94 58.021 5.86667 58.2277 5.72C58.4343 5.56667 58.5377 5.33 58.5377 5.01C58.5377 4.69 58.4343 4.45667 58.2277 4.31C58.021 4.15667 57.6943 4.08 57.2477 4.08H55.8277V5.94H57.2477Z"
                        fill="#FCFCFC"
                      />
                      <line opacity="0.15" x1="18.5" y1="2" x2="18.5" y2="12" stroke="#FCFCFC" />
                    </svg>
                  </span>
                </button>
              </li>

              <li class="mx-3">
                <span>
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="25"
                    height="31"
                    viewBox="0 0 25 31"
                    fill="none"
                  >
                    <ellipse cx="12.5345" cy="11.0095" rx="8.46888" ry="8.63826" fill="white" />
                    <path
                      d="M14.5193 12.7697H10.7415L9.96984 14.5665H8.16156L11.8933 6.44651H13.333L17.0647 14.5665H15.291L14.5193 12.7697ZM13.9319 11.4106L12.6304 8.36996L11.3289 11.4106H13.9319Z"
                      fill="#00B394"
                    />
                    <path
                      d="M22.7086 9.30867C22.5054 8.19077 23.1151 6.80188 22.5731 5.78561C22.0311 4.80322 20.5406 4.53222 19.6937 3.71921C18.8468 2.90619 18.5081 1.41567 17.4918 0.941415C16.4755 0.433282 15.0866 1.11079 13.9687 0.97529C12.8508 0.839788 11.6652 -0.176478 10.5812 0.0267756C9.46329 0.230029 8.75191 1.58505 7.73564 2.12706C6.75325 2.66907 5.22885 2.53356 4.41584 3.34658C3.60283 4.19346 3.83996 5.71786 3.33183 6.70025C2.82369 7.71652 1.53642 8.52953 1.36705 9.64742C1.23154 10.7653 2.28168 11.8832 2.48494 13.0011C2.68819 14.119 2.07843 15.5079 2.62044 16.5242C3.16245 17.5065 4.65297 17.7775 5.49986 18.5906C6.34675 19.4036 6.6855 20.8941 7.70177 21.3684C8.71803 21.8765 10.1069 21.199 11.2248 21.3345C12.3427 21.47 13.5284 22.4862 14.6124 22.283C15.7303 22.0797 16.4417 20.7247 17.4579 20.1827C18.4403 19.6407 19.9647 19.7762 20.7777 18.9632C21.5907 18.1163 21.3536 16.5919 21.8279 15.6095C22.336 14.5933 23.6233 13.7802 23.7926 12.6623C23.962 11.5445 22.9119 10.4266 22.7086 9.30867ZM12.6137 18.5567C8.54866 18.5567 5.22886 15.2369 5.22886 11.1718C5.22886 7.10676 8.54866 3.78696 12.6137 3.78696C16.6788 3.78696 19.9986 7.10676 19.9986 11.1718C19.9647 15.2708 16.6788 18.5567 12.6137 18.5567Z"
                      fill="#00B394"
                    />
                    <path
                      d="M19.0379 20.928C18.6314 21.0296 18.2249 21.0973 17.9878 21.2328C17.7168 21.3683 17.4458 21.6732 17.107 21.9781C16.5311 22.554 15.7859 23.2654 14.7696 23.4686C14.6002 23.5025 14.4308 23.5025 14.2276 23.5025C13.9566 23.5025 13.6856 23.4686 13.4146 23.4009L16.9376 30.176L19.7832 25.8399L25 26.0093L21.7141 19.6407C21.6802 19.6746 21.6802 19.7084 21.6463 19.7084C20.9011 20.5215 19.8848 20.7247 19.0379 20.928Z"
                      fill="#00B394"
                    />
                    <path
                      d="M10.8063 22.4863C10.5353 22.4863 10.2304 22.5202 9.89165 22.5879C9.45127 22.6557 9.01089 22.7234 8.57051 22.7234C7.99462 22.7234 7.52036 22.6218 7.07998 22.4185C6.13147 21.9782 5.65721 21.1313 5.21683 20.386C4.9797 20.0134 4.77645 19.6408 4.53932 19.4036C4.33607 19.2342 4.03119 19.0649 3.69243 18.8616L0 25.9755L5.18295 25.7722L8.06237 30.176L11.8903 22.7912C11.5516 22.6557 11.2467 22.5202 11.0095 22.4863C10.9418 22.4863 10.874 22.4863 10.8063 22.4863Z"
                      fill="#00B394"
                    />
                  </svg>
                </span>
              </li>

              <li class="mx-3">
                <img :src="user.path"  alt='user' />
              </li>
              <li>
                {{ user.name}}
                <br />
                <span>{{user.email}}</span>
              </li>

              <li class="mx-3">
                <span>
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="10"
                    height="7"
                    viewBox="0 0 10 7"
                    fill="none"
                  >
                    <path
                      d="M1.44678 1.625L5.19678 5.375L8.94678 1.625"
                      stroke="#2D2D2D"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </span>
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
      user: {
        path: "../../assets/Vectors/user1.png",
        name: "Chioma Davis",
        email: "Chioma@natterbase",
      },
    };
  },
};
</script>
<style scoped>
@import url(//netdna.bootstrapcdn.com/font-awesome/4.0.3/css/font-awesome.css);
header {
  width: 100%;
  background: #fbfbfb;
  padding: 8px 0px;
}

.nav-item {
  font-family: "Poppins", sans-serif;
  color: #000000;
  font-weight: 600;
  font-size: 14px;
  line-height: 19px;
  font-style: normal;
}
.actives {
  background: green;
}
.search__area {
  display: flex;
  flex-direction: row;
}
.bg-inherit {
  background: inherit;
}
.input-group
  > .input-group-append:last-child
  > .btn:not(:last-child):not(.dropdown-toggle),
.input-group
  > .input-group-append:last-child
  > .input-group-text:not(:last-child),
.input-group > .input-group-append:not(:last-child) > .btn,
.input-group > .input-group-append:not(:last-child) > .input-group-text,
.input-group > .input-group-prepend > .btn,
.input-group > .input-group-prepend > .input-group-text {
  border: none;
  cursor: pointer;
}
.input-group > .custom-select:not(:first-child),
.input-group > .form-control:not(:first-child) {
  border: none;
  background: inherit;
}
.owner__btn {
  background: linear-gradient(0deg, #4dbd98, #4dbd98),
    linear-gradient(0deg, #4dbd98, #4dbd98),
    linear-gradient(0deg, #4dbd98, #4dbd98), #4dbd98;
  border-radius: 5px;
  border: none;
  padding: 1px 5px;
}
.owner__btn:focus,
[type="button"]:focus {
  outline: none;
}

input[type="search"]:focus {
  border-color: #f9f9f9;
  box-shadow: none;
  outline: 0 none;
  border: 1px solid rgba(0, 0, 0, 0.15);
}
</style>
