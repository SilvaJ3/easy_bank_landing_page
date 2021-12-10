<template>
  <section>
    <div class="section3 flex flex-col pt-24 pb-12 px-32">
      <h1 class="text-4xl">Latest Articles</h1>
      <div class="flex justify-evenly items-center my-20">
        <div class="flex flex-col justify-start items-start mr-6 bg-white rounded-xl overflow-hidden" v-for="(article, index) in articles" :key="index">
          <div clss="h-1/2 overflow-hidden">
            <img :src="article.img" alt="" class="w-full">
          </div>
          <div class="flex flex-col p-5 h-1/2">
            <span class="text-xs">By {{ article.author }}</span>
            <h1 class="text-lg mb-2">{{ article.title }}</h1>
            <p class="text-sm">{{ article.body }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import currency from "../assets/images/image-currency.jpg"
import restaurant from "../assets/images/image-restaurant.jpg"
import plane from "../assets/images/image-plane.jpg"
import confetti from "../assets/images/image-confetti.jpg"

export default {
  name: "Section3",
  data(){
    return {
      articles: [
        {
          img: currency,
          author: "Claire Robinson",
          title: "Receive money in any currency with no fees",
          body: "The world is getting smaller and we’re becoming more mobile. So why should you be forced to only receive money in a single …",
        },
        {
          img: restaurant,
          author: "Wilson Hutton",
          title: "Treat yourself without worrying about money",
          body: "Our simple budgeting feature allows you to separate out your spending and set realistic limits each month. That means you …",
        },
        {
          img: plane,
          author: "Wilson Hutton",
          title: "Take your Easybank card wherever you go",
          body: "We want you to enjoy your travels. This is why we don’t charge any fees on purchases while you’re abroad. We’ll even show you …",
        },
        {
          img: confetti,
          author: "Claire Robinson",
          title: "Our invite-only Beta accounts are now live!",
          body: "After a lot of hard work by the whole team, we’re excited to launch our closed beta. It’s easy to request an invite through the site ...",
        },

      ]
    }
  }
}
</script>

<style scoped>
.section3 {
  background-color: #fafafa;
}

.section3 span, .section3 p {
  color: hsl(233, 8%, 62%)
}

.section3 img{
  width: 276px;
  height: 184px
}
</style>