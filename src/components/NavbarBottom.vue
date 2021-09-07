<template>
  <nav id="navbar-bottom">
    <ul>
      <li v-for="(image, index) in images" :key="index">
        <!-- <img :src="getImg(image.img)" :alt="image.text" /> -->
        <a :href="image.url">{{ image.text }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavbarBottom",
  data() {
    return {
      images: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital comics",
          url: "#",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "Dc merchandise",
          url: "#",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Subscription",
          url: "#",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "Comics shop locator",
          url: "#",
        },
        {
          img: "buy-comics-dc-power-visa.png",
          text: "Dc power visa",
          url: "#",
        },
      ],
    };
  },
  // methods: {
  //   getImg(path) {
  //     return require("@/assets/img/" + path);
  //   },
  // },
};
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
      a {
        color:$font-white;
        text-transform: $text-size-up;
        padding: 20px;
      }
    }
}
</style>