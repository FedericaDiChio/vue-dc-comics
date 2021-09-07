<template>
  <div id="app">
    <Header />
    <Products />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Products from "./components/Products.vue"

export default {
  name: 'App',
  components: {
    Header,
    Products,
  }
}
</script>

<style lang="scss">
#app {
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  .container {
        max-width: 1200px;
        margin: 0 auto;
    }

  img {
    max-width: 100%;
    height: auto;
  }

  li {
    list-style-type: none;
    padding: 10px; 
  }

  li a {
    text-decoration: none;
  }
}
</style>
