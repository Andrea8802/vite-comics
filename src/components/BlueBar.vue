<script>
export default {
    name: "BlueBar",
    data() {
        return {
            blueBarContent: [
                {
                    name: "DIGITAL COMICS",
                    image: "buy-comics-digital-comics.png"
                },

                {
                    name: "DC MERCHANDISE",
                    image: "buy-comics-merchandise.png"
                },

                {
                    name: "SUSCRIPTION",
                    image: "buy-comics-subscriptions.png"
                },

                {
                    name: "COMIC SHOP LOCATION",
                    image: "buy-comics-shop-locator.png"
                },

                {
                    name: "DC POWER VISA",
                    image: "buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <ul>
            <li v-for="item in blueBarContent">
                <img :src="'./src/assets/img/' + item.image" alt="">
                <span>
                    {{ item.name }}
                </span>
            </li>
        </ul>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables.scss" as *;
@use "../assets/styles/partials/mixins.scss" as *;


section {
    background-color: $primary-color;
    height: 120px;
    width: 100%;
    color: white;
    padding: 0 220px;
    position: relative;
    z-index: 2;

    ul {
        height: 100%;
        @include d-flex (evenly);

        li {
            height: 100%;
            @include d-flex (center);
            gap: 10px;
            font-size: 10px;

            img {
                height: 35%;
                max-width: 30%;
            }

            span {
                cursor: pointer;

                &:hover {
                    text-decoration: underline;
                }
            }

        }
    }
}
</style>