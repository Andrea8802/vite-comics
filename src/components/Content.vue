<script>
import ListCard from '../components/ListCard.vue'

export default {
    name: "Content",
    components: {
        ListCard
    },

    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="jumbotron">

    </div>
    <section>
        <ListCard />
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
    display: flex;
    align-items: center;
    font-weight: bold;
    font-size: 24px;
}
</style>