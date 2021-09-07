<template>
  <footer>
    <div class="container">
      <section id="main-footer">
        <div class="row">
          <div class="col">
            <ul>
              <h4>dc comics</h4>
              <li v-for="(comic, index) in comics" :key="index">
                <a href="comic.url">{{ comic.text }}</a>
              </li>
            </ul>
            <ul>
              <h4>shop</h4>
              <li v-for="(shop, index) in shops" :key="index">
                <a href="shop.url">{{ shop.text }}</a>
              </li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <h4>dc</h4>
              <li v-for="(copyright, index) in copyrights" :key="index">
                <a href="copyright.url">{{ copyright.text }}</a>
              </li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <h4>sites</h4>
              <li v-for="(site, index) in sites" :key="index">
                <a href="site.url">{{ site.text }}</a>
              </li>
            </ul>
          </div>
        </div>
      </section>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MainFooter",
  data() {
    return {
      comics: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
      ],
      shops: [
        {
          text: "Shop DC",
          url: "#",
        },
        {
          text: "Shop DC Collectibles",
          url: "#",
        },
      ],
      copyrights: [
        {
          text: "terms of use",
          url: "#",
        },
        {
          text: "privacy policy(new)",
          url: "#",
        },
        {
          text: "ad choices",
          url: "#",
        },
        {
          text: "advertising",
          url: "#",
        },
        {
          text: "jobs",
          url: "#",
        },
        {
          text: "subscriptions",
          url: "#",
        },
        {
          text: "talent workshops",
          url: "#",
        },
        {
          text: "CPSC certificates",
          url: "#",
        },
        {
          text: "ratings",
          url: "#",
        },
        {
          text: "shop help",
          url: "#",
        },
        {
          text: "contact us",
          url: "#",
        },
      ],
      sites: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD magazine",
          url: "#",
        },
        {
          text: "DC kids",
          url: "#",
        },
        {
          text: "DC universe",
          url: "#",
        },
        {
          text: "DC power visa",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/assets/styles/_vars.scss";

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