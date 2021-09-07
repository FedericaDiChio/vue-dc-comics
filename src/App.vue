<template>
  <div id="app">
    <Header />
    <Products />
    <NavbarBottom />
    <MainFooter />
    <BottomFooter />
  </div>  
</template>

<script>
import Header from './components/Header.vue'
import Products from "./components/Products.vue"
import NavbarBottom from "./components/NavbarBottom.vue"
import MainFooter from "./components/MainFooter.vue"
import BottomFooter from "./components/BottomFooter.vue"

export default {
  name: 'App',
  components: {
    Header,
    Products,
    NavbarBottom,
    MainFooter,
    BottomFooter,
  }
}
</script>

<style lang="scss">
  @import "@/assets/styles/style.scss";
</style>
