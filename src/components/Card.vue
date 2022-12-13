<script>
export default {
    name: "Card",
    props: {
        details: Object
    }
}
</script>

<template>
    <div class="card">
        <img :src="details.thumb" alt="">
        <div class="text">
            {{ details.series }}
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    height: 250px;
    width: 180px;


    img {
        max-height: 80%;
        max-width: 100%;
    }

    .text {
        max-height: 20%;
        max-width: 100%;
        font-size: 14px;
        font-weight: normal;
    }
}
</style>