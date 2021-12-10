<template>
  <div id="app" class="h-full w-full overflow-x-hidden">
    <Header/>
    <Section1/>
    <Section2/>
    <Section3/>
    <Footer/>
  </div> 
</template>

<script>
import logo from "./assets/images/logo.svg"
import Header from "./components/Header.vue"
import Section1 from "./components/Section1.vue"
import Section2 from "./components/Section2.vue"
import Section3 from "./components/Section3.vue"
import Footer from "./components/Footer.vue"

export default {
  name: 'App',
  data() {
    return {
      logo: logo
    }
  },
  components: {
    Header,
    Section1,
    Section2,
    Section3,
    Footer,
  }
}
</script>

<style>
#app {
  font-family: 'Public Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}


</style>
