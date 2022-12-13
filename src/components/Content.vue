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
    <div class="jumbotron"></div>
    <section>
        <ListCard />
        <div class="load">
            <button>
                LOAD MORE
            </button>
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
    min-height: 100px;
    width: 100%;
    color: white;

    .load {
        @include d-flex(center);

        button {
            background-color: $primary-color;
            border: none;
            color: white;
            font-weight: bold;
            padding: 10px 30px;
            margin-bottom: 30px;
        }
    }

}
</style>