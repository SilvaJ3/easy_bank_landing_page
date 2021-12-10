<template>
  <footer>
    <div class="footer px-32 py-16 flex justify-between">
      <div clas="flex flex-col justify-between items-center w-full">
        <div class="flex">
          <img :src="logo" alt="" fill="white" class="text-white mb-10">
          <!-- <h1 class="m-0 font-bold">easybank</h1> -->
        </div>
        <div class="flex">
          <img :src="facebook" alt="" class="mr-2">
          <img :src="youtube" alt="" class="mr-2">
          <img :src="twitter" alt="" class="mr-2">
          <img :src="pinterest" alt="" class="mr-2">
          <img :src="instagram" alt="" class="mr-2">
        </div>
      </div>
      <div class="flex justify-between mr-20">
        <ul class="text-white list-none mr-20">
          <li class="mb-3">About Us</li>
          <li class="mb-3">Contact</li>
          <li class="mb-3">Blog</li>
        </ul>
        <ul class="text-white list-none">
          <li class="mb-3">Careers</li>
          <li class="mb-3">Support</li>
          <li class="mb-3">Privacy Policy</li>
        </ul>
      </div>
      <div class="flex flex-col items-end justify-center">
        <div class="rounded-full px-5 py-2 cursor-pointer header_button">
          <span class="pointer-events-none text-white font-bold text-sm">Request Invite</span>
        </div>
        <span class="text-right copyright text-sm mt-5">© Easybank. All Rights Reserved</span>
      </div>
    </div>
  </footer>
</template>

<script>
import logo from "../assets/images/logo.svg"
import facebook from "../assets/images/icon-facebook.svg"
import youtube from "../assets/images/icon-youtube.svg"
import twitter from "../assets/images/icon-twitter.svg"
import pinterest from "../assets/images/icon-pinterest.svg"
import instagram from "../assets/images/icon-instagram.svg"

export default {
  name: "Footer",
  data(){ 
    return {
      logo: logo,
      facebook: facebook,
      youtube: youtube,
      twitter: twitter,
      pinterest: pinterest,
      instagram: instagram,
    }
  }
}
</script>

<style scoped>
.footer {
  background-color: hsl(233, 26%, 24%)
}

.header_button {
  background: linear-gradient(to left, hsl(192, 70%, 51%) , hsl(136, 65%, 51%));
}

.copyright {
  color: hsl(233, 8%, 62%)
}
</style>