<template>
    <div class="card">
        <figure>
            <img :src="img" alt="" />
        </figure>
        <address>
            {{ series }}
        </address>
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
        padding: 15px;
        flex-basis: 15%;
        address {
            font-style: normal;
        }
                
}
    
</style>