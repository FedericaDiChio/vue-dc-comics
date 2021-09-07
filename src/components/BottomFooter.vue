<template>  
    <section id="bottom-footer">
        <div class="container">
            <div class="row">
                <div class="col">
                    <p>sign-up now!</p>
                </div>
                <div class="col">
                    <ul id="footer-icons">
                        <p>follow us</p>
                        <li v-for="(icon, index) in icons" :key="index">
                            <a href=""><img :src="getImg(icon.image)" alt=""></a>
                        </li>
                    </ul>                    
                </div>
            </div>
        </div>
    </section>  
</template>

<script>
export default {
    name: "BottomFooter",
    data() {
        return {
            icons: [
            {
                image: "footer-facebook.png"
            },
            {
                image: "footer-twitter.png"
            },
            {
                image: "footer-youtube.png"
            },
            {
                image: "footer-pinterest.png"
            },
            {
                image: "footer-periscope.png"
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
    #bottom-footer {        
        background-color: rgb(48, 48, 48);
        .row {
               justify-content: space-between;
        align-items: center;
            #footer-icons {
                display: flex;
                align-items: center;
    }
        }
    }
    
</style>