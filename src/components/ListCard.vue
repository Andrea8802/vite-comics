<script>
import Card from '../components/Card.vue'
import json from '../assets/dc-comics.json'

export default {
    name: "ListCard",
    components: {
        Card
    },
    data() {
        return {
            cards: json
        }
    }
}
</script>

<template>
    <div class="list">
        <Card v-for="(card, indice) in cards" :key="indice" :details="card" />
    </div>

</template>

<style lang="scss" scoped>
@use '../assets/styles/partials/mixins.scss' as *;

.list {
    width: 75%;
    margin: 0 auto;
    padding: 30px 0;
    @include d-flex(center);
    flex-wrap: wrap;
    row-gap: 30px;
}
</style>