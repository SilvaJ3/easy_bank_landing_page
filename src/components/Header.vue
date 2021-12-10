<template>
  <header>
      <nav class="w-full flex justify-evenly items-center py-5 z-10 relative bg-white">
        <div>
          <img :src="logo" alt="">
        </div>
        <div>
          <ul class="flex justify-center items-center list-none">
            <li class="mx-2">Home</li>
            <li class="mx-2">About</li>
            <li class="mx-2">Contact</li>
            <li class="mx-2">Blog</li>
            <li class="mx-2">Careers</li>
          </ul>
        </div>
        <div>
          <div class="rounded-full px-5 py-2 cursor-pointer header_button">
            <span class="pointer-events-none text-white font-bold text-sm">Request Invite</span>
          </div>
        </div>
      </nav>
    </header>
</template>

<script>
import logo from "../assets/images/logo.svg"

export default {
  name: "Header",
  data() {
    return {
      logo: logo
    }
  }
}
</script>

<style scoped>

.header_button {
  background: linear-gradient(to left, hsl(192, 70%, 51%) , hsl(136, 65%, 51%));
}

</style>