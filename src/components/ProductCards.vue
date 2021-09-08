<template>
    <div class="card">
        <figure>
            <img :src="img" alt="" />
        </figure>
        
        <p>{{ series }}</p>
    </div>
</template>

<script>
export default {
    name: "ProductCards",
    props: ["img", "series"]
}
</script>

<style lang="scss">
    .card {
        
        flex-basis: 15%;
        // text-align: center;
                
}
    
</style>