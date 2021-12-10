<template>
  <section>
    <div class="flex flex-col pt-24 pb-12 px-32 section2">
      <div>
        <h1 class="text-4xl mb-5">Why choose Easybank?</h1>
        <p class="w-1/2">We leverage Open Banking to turn your bank account into your financial hub. Control your finances like never before.</p>
      </div>
      <div class="flex justify-center items-center my-20">
        <div class="flex flex-col justify-start items-start mr-3" v-for="(service, index) in services" :key="index">
          <img :src="service.img" alt="">
          <h1 class="my-5 text-xl">{{ service.title }}</h1>
          <p class="pr-10">{{ service.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import online from "../assets/images/icon-online.svg"
import budgeting from "../assets/images/icon-budgeting.svg"
import onboarding from "../assets/images/icon-onboarding.svg"
import api from "../assets/images/icon-api.svg"

export default {
  name: "Section2",
  data(){
    return {
      services: [
        {
          img: online,
          title: "Online Banking",
          description: "Our modern web and mobile applications allow you to keep track of your finances wherever you are in the world.",
        },
        {
          img: budgeting,
          title: "Simple Budgeting",
          description: "See exactly where your money goes each month. Receive notifications when you’re close to hitting your limits.",
        },
        {
          img: onboarding,
          title: "Fast Onboarding",
          description: "We don’t do branches. Open your account in minutes online and start taking control of your finances right away.",
        },
        {
          img: api,
          title: "Open API",
          description: "Manage your savings, investments, pension, and much more from one account. Tracking your money has never been easier.",
        },
      ]
    }
  }
}
</script>

<style scoped>
.section2 {
  background-color: #f4f5f7

}

.section2 p {
  color: hsl(233, 8%, 62%)
}
</style>