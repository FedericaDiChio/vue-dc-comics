<template>
  <section id="products">
      <main>
          <p>content goes here</p> 
      </main>
  </section>
  
</template>

<script>
export default {
    name: "Products",
}
</script>

<style lang="scss">
@import "@/assets/styles/_vars.scss";
    #products {
        height: 150px;
        background-color: rgb(0,0,0);
            p {
                line-height: 150px;
                text-align: center;
                color: $font-white;
                text-transform:$text-size-up;
            }
    }


</style>