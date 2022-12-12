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
