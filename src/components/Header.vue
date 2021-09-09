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

<style lang="scss" scoped>
@import "../assets/styles/_vars.scss";
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100px;
  background-color: $font-white;

    #header-logo {
      max-width: 60px;
    } 
}

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
</style>