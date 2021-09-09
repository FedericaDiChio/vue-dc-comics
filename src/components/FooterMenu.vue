<template>
  <ul>
    <h4>{{ menu.title }}</h4>
    <li v-for="(link, index) in menu.links" :key="index">
      <a href="link.url">{{ link.text  }}</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "FooterMenu",
  props: ["menu"],
};
</script>

<style>
</style>