<script>
import ListCard from '../components/ListCard.vue'

export default {
    name: "Content",
    components: {
        ListCard
    }
}
</script>

<template>
    <section class="jumbotron"></section>
    <section>
        <ListCard />
        <div class="load">
            <button>
                LOAD MORE
            </button>
        </div>

        <div class="title">
            CURRENT SERIES
        </div>
    </section>


</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables.scss" as *;
@use "../assets/styles/partials/mixins.scss" as *;

.jumbotron {
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
    height: 300px;
}

section {
    background-color: #1c1c1c;
    min-height: 700px;
    width: 100%;
    color: white;
    position: relative;


    .load {
        @include d-flex(center);

        button {
            background-color: $primary-color;
            border: none;
            color: white;
            font-weight: bold;
            padding: 10px 30px;

            &:hover {
                background-color: transparent;
                border: 3px solid $primary-color;
                padding: 8px 30px;

            }
        }
    }

    .title {
        background-color: $primary-color;
        color: white;
        font-weight: bold;
        padding: 12px 20px;
        font-size: 18px;
        position: absolute;
        top: -25px;
        left: 215px;

    }



}
</style>