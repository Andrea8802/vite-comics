<script>

export default {
    name: "Header",
    data() {
        return {
            logoImage: "./src/assets/img/dc-logo.png",
            navItems: [
                {
                    name: "CHARACTERS",
                    active: true,
                    link: "#"
                },

                {
                    name: "COMICS",
                    active: false,
                    link: "#"
                },

                {
                    name: "MOVIES",
                    active: false,
                    link: "#"
                },

                {
                    name: "TV",
                    active: false,
                    link: "#"
                },

                {
                    name: "GAMES",
                    active: false,
                    link: "#"
                },

                {
                    name: "COLLECTIBLES",
                    active: false,
                    link: "#"
                },

                {
                    name: "VIDEOS",
                    active: false,
                    link: "#"
                },

                {
                    name: "FANS",
                    active: false,
                    link: "#"
                },

                {
                    name: "NEWS",
                    active: false,
                    link: "#"
                },

                {
                    name: "SHOP",
                    active: false,
                    link: "#"
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
            <li v-for="(item, n) in navItems" :class="{ itemSelected: item.active }" :key="n">
                <a href="#">
                    {{ item.name }}
                </a>
            </li>
        </ul>
    </header>


</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables.scss" as *;
@use "../assets/styles/partials/mixins.scss" as *;


.itemSelected {
    border-bottom: 5px solid $primary-color;

    a {
        color: $primary-color;

    }

    &:hover {
        border: none;
    }
}

header {
    @include d-flex (between);
    height: 100px;
    width: 100%;
    padding: 0 260px;

    img {
        height: 65%;
    }

    ul {
        @include d-flex (evenly);
        gap: 20px;

        li a {
            padding: 42px 0;
            text-decoration: none;
            color: black;
            display: inline-block;
            font-size: 10px;
            font-weight: bold;

            &:hover {
                border-bottom: 5px solid $primary-color;
                color: $primary-color;
            }
        }
    }

}
</style>
