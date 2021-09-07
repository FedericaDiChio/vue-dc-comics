<template>
  <nav id="navbar-bottom">
    <ul>
      <li v-for="(icon, index) in icons" :key="index">
        <img :src="getImg(icon.icon)" alt="icon.text" />
        <a href="">{{ icon.text }} </a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavbarBottom",
  data(){
    return{
      icons: [
        {
          icon: "buy-comics-digital-comics.png",
          text: "digital comics"
        },
        {
          icon: "buy-comics-merchandise.png",
          text: "DC merchandise"
        },
        {
          icon: "buy-comics-shop-locator.png",
          text: "comic shop locator"
        },
        {
          icon: "buy-comics-subscriptions.png",
          text: "subscriptions"
        },
        {
          icon: "buy-dc-power-visa.svg",
          text: "DC power visa"
        },

      ]
    }
  },

  methods: {
      getImg(path){
          return require ("@/assets/img/" + path);
      }
  }
}
</script>
    
<style lang="scss">
@import "@/assets/styles/_vars.scss";
#navbar-bottom {
  height: 170px;
  background-color: $color-blue;
  display:flex;
  justify-content: center;
  align-items:center;
  ul {
      display: flex;  
      li {
        display: flex;
        justify-content: center;
        align-items: center;
          a {
            color:$font-white;
            text-transform: $text-size-up;
            margin-right: 30px;
          }
          img {
            margin-right: 10px;
            width: 40px;
          }
      }    
    }
}

</style>