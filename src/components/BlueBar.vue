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
                {{ item.name }}
            </li>
        </ul>
    </section>
</template>

<style scoped>
section {
    background-color: #0282f9;
    height: 120px;
    width: 100%;
    color: white;
    padding: 0 220px;
    position: relative;
    z-index: 2;
}

ul {
    height: 100%;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}

li {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    font-size: 10px;
}

ul li img {
    height: 35%;
    max-width: 30%;
}
</style>