<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style lang="scss">
#app {
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  // .container {
  //       max-width: 1200px;
  //       margin: 0 auto;
  //   }

  img {
    max-width: 100%;
    height: auto;
  }

  li {
    list-style-type: none;
  }

  li a {
    text-decoration: none;
  }
}
</style>
