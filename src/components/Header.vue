<template>
  <div class="container">
    <header>
      <figure id="header-logo">
        <img src="@/assets/img/dc-logo.png" alt="logo" />
      </figure>
      <nav id="navbar-top">
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
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
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/assets/styles/_vars.scss";
header {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
    ul {
      display: flex;
      li {
        padding: 10px;
      }      
        a {
          font-size: 15px;
          color: $color-black;
          text-transform:$text-size-up;
        }
    }
}

</style>