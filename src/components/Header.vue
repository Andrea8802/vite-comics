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
                <a href="#">
                    {{ item.name }}
                </a>
            </li>
        </ul>
    </header>


</template>

<style scoped>
.itemSelected {
    border-bottom: 5px solid #0282f9;
}

.itemSelected>a {
    color: #0282f9;
}

.itemSelected:hover {
    border: none;
}

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
}

header li a {
    padding: 42px 0;
    text-decoration: none;
    color: black;
    display: inline-block;
    font-size: 10px;
    font-weight: bold;
}

header li a:hover {
    border-bottom: 5px solid #0282f9;
    color: #0282f9;
}
</style>
