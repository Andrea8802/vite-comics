<script>

export default {
    name: "Header",
    data() {
        return {
            logoImage: "./src/assets/img/dc-logo.png",
            navItems: [
                {
                    name: "CHARACTERS",
                    active: true
                },

                {
                    name: "COMICS",
                    active: false
                },

                {
                    name: "MOVIES",
                    active: false
                },

                {
                    name: "TV",
                    active: false
                },

                {
                    name: "GAMES",
                    active: false
                },

                {
                    name: "COLLECTIBLES",
                    active: false
                },

                {
                    name: "VIDEOS",
                    active: false
                },

                {
                    name: "FANS",
                    active: false
                },

                {
                    name: "NEWS",
                    active: false
                },

                {
                    name: "SHOP",
                    active: false
                },
            ]
        }
    }
}
</script>

<template>

    <header>
        <img :src="logoImage" alt="">
        <ul>
            <li v-for="item in navItems" :class="{ itemSelected: item.active }">
                {{ item.name }}
            </li>
        </ul>
    </header>


</template>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
    width: 100%;
    padding: 0 260px;
}

header img {
    height: 65%;
}

header ul {
    display: flex;
    justify-content: space-evenly;
    align-self: center;
    gap: 20px;
    font-size: 10px;
    font-weight: bold;
}
</style>
