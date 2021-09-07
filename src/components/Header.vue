<template>
  <header>
    <figure id="header-logo">
      <img src="@/assets/dc-logo.png" alt="logo" />
    </figure>
    <nav id="navbar">
      <ul>
        <li v-for="(link, index) in links" :key="index">
            <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
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
header {
  height: 100px;
//   background-color: royalblue;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

#header-logo {
    max-width: 70px;
}

#navbar ul {
    display: flex;
}

a {
    color: black;
       
}
</style>