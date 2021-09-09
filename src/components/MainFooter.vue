<template>
  <footer>
    <div class="container">
      <section id="main-footer">
        <div class="row">
          <div v-for="(menu, index) in footerMenu" :key="index" class="col">
            <FooterMenu :menu="menu" />
          </div>
        </div>
      </section>
    </div>
  </footer>
</template>

<script>
import FooterMenu from "@/components/FooterMenu.vue";
export default {
  name: "MainFooter",
  data() {
    return {
      footerMenu: [
        {
          title: "DC comics",
          links: [
              { text: "Characters", url: "#"},
              { text: "Comics",url: "#"},
              { text: "Movies", url: "#"},
              { text: "TV", url: "#"},
              { text: "Games", url: "#"},
              { text: "Videos", url: "#"},
              { text: "News", url: "#"},
          ],
        },
        {
            title: "shops",
            links: [
                { text: "Shop DC", url: "#"},
                { text: "Shop DC Collectibles",url: "#"},

            ],
        },
        {
            title: "DC",
            links: [
                { text: "terms of use", url: "#"},
                { text: "privacy policy(new)",url: "#"},
                { text: "ad choices", url: "#"},
                { text: "advertising", url: "#"},
                { text: "jobs", url: "#"},
                { text: "subscriptions", url: "#"},
                { text: "CPSC certificates", url: "#"},
                { text: "ratings", url: "#"},
                { text: "shop help", url: "#"},
                { text: "contact us", url: "#"},
            ],
          },
          {
            title: "sites",
            links: [
                { text: "DC", url: "#"},
                { text: "MAD magazine",url: "#"},
                { text: "DC kids", url: "#"},
                { text: "DC universe", url: "#"},
                { text: "DC universe", url: "#"},
                { text: "DC power visa", url: "#"},

            ],
          } 
      ],  
    }
  },    
  components: { FooterMenu },
};  
</script>

<style lang="scss">
@import "../assets/styles/_vars.scss";

#main-footer {
  height: 400px;
  background-image: url("../assets/img/dc-logo-bg.png");
  background-size: auto;
  background-repeat: no-repeat;
  background-position: right;
}

  .col {
    padding: 30px;
    h4 {
      color: $font-white;
      font-size: 18px;
      text-transform: $text-size-up;
    }
}

a {
  color: grey;
  text-transform: $text-size-cap;
}
</style>