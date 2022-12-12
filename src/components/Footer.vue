<script>
export default {
    name: "Footer",
    data() {
        return {
            logoImageBg: "./src/assets/img/dc-logo-bg.png",
            linkFooter: {

                dcComics: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "TV",
                    "Games",
                    "Videos",
                    "News"
                ],



                dC: [
                    "Term Of Use",
                    "Privacy policy (New)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact US"
                ],



                sites: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa"
                ],



                shop: [
                    "Shop DC",
                    "Shop DC Collectibles"
                ]


            }
        }
    }
}
</script>

<template>
    <footer>
        <section class="top">
            <div class="left">
                <div class="list">
                    DC COMICS
                    <ul>
                        <li v-for="link in linkFooter.dcComics">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                </div>

                <div class="list">
                    DC
                    <ul>
                        <li v-for="link in linkFooter.dC">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                </div>

                <div class="list">
                    SITES
                    <ul>
                        <li v-for="link in linkFooter.sites">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                </div>

                <!-- A CAPO -->
                <div class="list">
                    SHOP
                    <ul>
                        <li v-for="link in linkFooter.shop">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="right">
                <img :src="logoImageBg" alt="">
            </div>
        </section>

        <section class="bottom">
            <a href="#">
                SIGN-UP NOW!
            </a>

            <div>
                <span>FOLLOW US</span>
                <!-- ICONS -->
            </div>
        </section>
    </footer>
</template>

<style scoped>
footer {
    width: 100%;
    height: calc(100vh - 320px);
    position: relative;
}

.top {
    background-image: url("./src/assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    padding: 80px 250px;
    height: calc(100% - 90px);
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.left {
    display: flex;
    flex-wrap: wrap;
    width: 40%;
    column-gap: 30px;
    color: white;
    font-size: 14px;
    font-weight: bold;
}

.left ul {
    font-size: 10px;
}

.left ul li {
    margin: 4px 0;
}

.left ul li a {
    text-decoration: none;
    color: gray;

}

.right img {
    width: 30%;
    position: absolute;
    top: -80px;
    right: 250px;
    z-index: 1;
}

.bottom {
    background-color: #303030;
    width: 100%;
    height: 90px;
    padding: 0 250px;
    position: relative;
    z-index: 2;
    display: flex;
    justify-content: space-between;
    align-items: center;

}
</style>