<template>
    <nav id="navbar-bottom">
        <ul>
            <!-- <li v-for="(image, index) in images" :key="index">
                <a :href="image.url">{{ image.text }}</a>
            </li> -->
        </ul>
    </nav>
</template>

<script>
export default {
    name: "NavbarBottom",
    // data() {
    // return {
    //   images: [
    //     {
    //       img: "buy-comics-digital-comics.png",
    //       text: "Digital comics",
    //       url: "#",
    //     },
    //     {
    //       img: "buy-comics-merchandise.png",
    //       text: "Dc merchandise",
    //       url: "#",
    //     },
    //     {
    //       img: "buy-comics-subscriptions.png",
    //       text: "Subscription",
    //       url: "#",
    //     },
    //     {
    //       img: "buy-comics-shop-locator.png",
    //       text: "Comics shop locator",
    //       url: "#",
    //     },
    //     {
    //       img: "buy-comics-dc-power-visa.png",
    //       text: "Dc power visa",
    //       url: "#",
    //     }
    //   ],
    // };
  // },
}
</script>
    
<style lang="scss">
    #navbar-bottom{
        height: 170px;
        background-color: royalblue;   
    }
</style>