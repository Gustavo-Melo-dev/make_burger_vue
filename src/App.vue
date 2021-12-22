<template>
  <Navbar :logo="logo_burger" :description="alt_burger" />
  <router-view />
  <Footer :footer="footer_burger" />
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

export default {
  name: "App",
  components: {
    Navbar,
    Footer,
  },
  setup() {
    const logo_burger = '/img/logo.png';
    const alt_burger = 'Logo da hamburgueria';
    const footer_burger = 'Make Burger'

    return {
      logo_burger,
      alt_burger,
      footer_burger,
    }
  }
}
</script>

<style>
  * {
    font-family: Helvetica, sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>
