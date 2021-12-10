<template>
  <section>
    <div class="w-full section1 px-10 py-44">
      <div class="flex justify-center items-center">
        <div class="flex flex-col justify-start items-start px-20 w-1/2">
          <h1 class="text-5xl">
            Next generation <br />
            digital banking
          </h1>
          <p class="my-5 pr-4">
            Take your financial life online. Your Easybank account will be a
            one-stop-shop for spending, saving, budgeting, investing, and much
            more.
          </p>
          <div class="rounded-full px-5 py-2 cursor-pointer header_button">
            <span class="pointer-events-none text-white font-bold text-sm">Request Invite</span>
          </div>
        </div>
        <div class="flex flex-col justify-center items-center w-1/2 relative">
          <img :src="mockups" alt="" class="absolute left-40">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import mockups from "../assets/images/image-mockups.png"

export default {
  data(){
    return {
      mockups: mockups
    }
  }
};
</script>

<style scoped>
.section1 {
  background-image: url("../assets/images/bg-intro-desktop.svg");
  background-repeat: no-repeat;
  background-position-x: 450%;
  background-position-y: 0%;
  background-color: #fafafa

}

.header_button {
  background: linear-gradient(to left, hsl(192, 70%, 51%) , hsl(136, 65%, 51%));
} 
</style>