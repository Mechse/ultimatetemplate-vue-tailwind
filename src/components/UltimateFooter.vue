<template>
  <footer
    class="bg-black w-full border-t pin-b flex items-center justify-center sm:justify-around flex-wrap p-4"
  >
    <div class="social-media p-4">
      <div class="glowing-social w-full bg-white mb-4"></div>
      <div class="flex">
        <!-- FACEBOOK -->
        <a
          @mouseenter="socialColorFacebook=hoverSocial"
          @mouseleave="socialColorFacebook=socialColor"
          href="https://facebook.com"
        >
          <svg
            width="50"
            height="50"
            viewBox="0 0 50 50"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              :style="socialColorFacebook"
              d="M41.6797 6.25H8.32031C7.17773 6.25 6.25 7.17773 6.25 8.32031V41.6797C6.25 42.8223 7.17773 43.75 8.32031 43.75H25V28.9062H20.5176V23.4375H25V19.3945C25 14.5508 28.3594 11.9141 32.6855 11.9141C34.7559 11.9141 36.9824 12.0703 37.5 12.1387V17.1973H34.0527C31.6992 17.1973 31.25 18.3105 31.25 19.9512V23.4375H36.8555L36.123 28.9062H31.25V43.75H41.6797C42.8223 43.75 43.75 42.8223 43.75 41.6797V8.32031C43.75 7.17773 42.8223 6.25 41.6797 6.25Z"
              fill="#C4C4C4"
            ></path>
          </svg>
        </a>
        <!-- INSTAGRAM -->
        <a
          @mouseenter="socialColorInstagram=hoverSocial"
          @mouseleave="socialColorInstagram=socialColor"
          href="https://instagram.com"
        >
          <svg
            width="50"
            height="50"
            viewBox="0 0 50 50"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              :style="socialColorInstagram"
              d="M32.8125 9.375C34.8828 9.375 36.8457 10.1953 38.3301 11.6699C39.8145 13.1445 40.625 15.1172 40.625 17.1875V32.8125C40.625 34.8828 39.8047 36.8457 38.3301 38.3301C36.8555 39.8145 34.8828 40.625 32.8125 40.625H17.1875C15.1172 40.625 13.1543 39.8047 11.6699 38.3301C10.1855 36.8555 9.375 34.8828 9.375 32.8125V17.1875C9.375 15.1172 10.1953 13.1543 11.6699 11.6699C13.1445 10.1855 15.1172 9.375 17.1875 9.375H32.8125ZM32.8125 6.25H17.1875C11.1719 6.25 6.25 11.1719 6.25 17.1875V32.8125C6.25 38.8281 11.1719 43.75 17.1875 43.75H32.8125C38.8281 43.75 43.75 38.8281 43.75 32.8125V17.1875C43.75 11.1719 38.8281 6.25 32.8125 6.25Z"
              fill="#C4C4C4"
            ></path>
            <path
              :style="socialColorInstagram"
              d="M35.1562 17.1875C33.8574 17.1875 32.8125 16.1426 32.8125 14.8438C32.8125 13.5449 33.8574 12.5 35.1562 12.5C36.4453 12.5 37.5 13.5449 37.5 14.8438C37.5 16.1426 36.4453 17.1875 35.1562 17.1875ZM25 18.75C28.4473 18.75 31.25 21.5527 31.25 25C31.25 28.4473 28.4473 31.25 25 31.25C21.5527 31.25 18.75 28.4473 18.75 25C18.75 21.5527 21.5527 18.75 25 18.75ZM25 15.625C19.8242 15.625 15.625 19.8242 15.625 25C15.625 30.1758 19.8242 34.375 25 34.375C30.1758 34.375 34.375 30.1758 34.375 25C34.375 19.8242 30.1758 15.625 25 15.625Z"
              fill="#C4C4C4"
            ></path>
          </svg>
        </a>
        <!-- LINKEDIN -->
        <a
          @mouseenter="socialColorLinkedIn=hoverSocial"
          @mouseleave="socialColorLinkedIn=socialColor"
          href="https://linkedin.com"
        >
          <svg
            width="50"
            height="50"
            viewBox="0 0 50 50"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              :style="socialColorLinkedIn"
              d="M40.7422 6.25H9.45313C7.74414 6.25 6.25 7.48047 6.25 9.16992V40.5273C6.25 42.2266 7.74414 43.7402 9.45313 43.7402H40.7324C42.4512 43.7402 43.7402 42.2168 43.7402 40.5273V9.16992C43.75 7.48047 42.4512 6.25 40.7422 6.25ZM17.8711 37.5H12.5V20.8008H17.8711V37.5ZM15.3711 18.2617H15.332C13.6133 18.2617 12.5 16.9824 12.5 15.3809C12.5 13.75 13.6426 12.5 15.4004 12.5C17.1582 12.5 18.2324 13.7402 18.2715 15.3809C18.2715 16.9824 17.1582 18.2617 15.3711 18.2617ZM37.5 37.5H32.1289V28.3691C32.1289 26.1816 31.3477 24.6875 29.4043 24.6875C27.9199 24.6875 27.041 25.6934 26.6504 26.6699C26.5039 27.0215 26.4648 27.5 26.4648 27.9883V37.5H21.0938V20.8008H26.4648V23.125C27.2461 22.0117 28.4668 20.4102 31.3086 20.4102C34.834 20.4102 37.5 22.7344 37.5 27.7441V37.5Z"
              fill="#C4C4C4"
            ></path>
          </svg>
        </a>
      </div>
    </div>
    <div class="made-by p-4 flex items-center justify-center flex-wrap">
      <div class="mx-4 my-1">
        <img class="w-12" src="../assets/logo.png" alt>
      </div>
      <div class="text-white text-center">
        <p>Made by Maximilian Leodolter.</p>
        <p></p>
      </div>
    </div>
    <div
      class="links text-white sm:w-full lg:w-auto p-4 flex justify-center sm:justify-around flex-wrap"
    >
      <div class="lg:mx-6 my-4 sm:my-0">
        <div class="mb-1">
          <a>Tel.: 0000 XXXX XXX</a>
        </div>
        <div class="mb-1">
          <a>Email.: max.mustermann@x.x</a>
        </div>
        <div class="line-seperator my-4"></div>
        <address>Musterstraße 1, 0000 Musterstadt
          <br>Musterland
        </address>
      </div>
      <div class="wrapper flex mt-6 sm:my-0">
        <div class="mr-6 sm:mx-6">
          <div class="footer-link">
            <a>Home</a>
          </div>
          <div class="footer-link">
            <a>About Us</a>
          </div>
          <div class="footer-link">
            <a>Contact</a>
          </div>
        </div>
        <div class="mx-6">
          <div class="footer-link">
            <a>Datenschutz</a>
          </div>
          <div class="footer-link">
            <a>Impressum</a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "UltimateFooter",
  data() {
    return {
      socialColor: "fill: white",
      socialColorFacebook: "",
      socialColorInstagram: "",
      socialColorLinkedIn: "",
      hoverSocial: "fill: green"
    };
  },
  methods: {},
  mounted() {
    this.socialColorFacebook = this.socialColor;
    this.socialColorInstagram = this.socialColor;
    this.socialColorLinkedIn = this.socialColor;
  }
};
</script>

<style scoped>
.glowing-social {
  height: 2px;
  background-color: white;
  box-shadow: 1px 1px 25px 5px white;
}
.line-seperator {
  width: 25%;
  height: 1px;
  background-color: white;
}
.footer-link {
  cursor: pointer;
}
</style>
