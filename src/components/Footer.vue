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


            },

            iconsSocial: [
                {
                    name: "facebook.png"
                },

                {
                    name: "twitter.png"
                },

                {
                    name: "youtube.png"
                },

                {
                    name: "facebook.png"
                },

                {
                    name: "periscope.png"
                },
            ]
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
                        <li v-for="(link, a) in linkFooter.dcComics" :key="a">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                    SHOP
                    <ul>
                        <li v-for="(link, b) in linkFooter.shop" :key="b">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                </div>

                <div class="list">
                    DC
                    <ul>
                        <li v-for="(link, c) in linkFooter.dC" :key="c">
                            <a href="#">
                                {{ link }}
                            </a>
                        </li>
                    </ul>
                </div>

                <div class="list">
                    SITES
                    <ul>
                        <li v-for="(link, d) in linkFooter.sites" :key="d">
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

            <div class="follow">
                <span>FOLLOW US</span>
                <img v-for="(icon, i) in iconsSocial" :src="'./src/assets/img/footer-' + icon.name" :key="i">
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables.scss" as *;
@use "../assets/styles/partials/mixins.scss" as *;


footer {
    width: 100%;
    height: calc(100vh - 320px);
    position: relative;

    .top {
        background-image: url("./src/assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        padding: 80px 250px;
        height: calc(100% - 90px);
        @include d-flex (between);

        .left {
            display: flex;
            flex-wrap: wrap;
            width: 40%;
            column-gap: 30px;
            color: white;
            font-size: 14px;
            font-weight: bold;

            ul {
                font-size: 10px;
                margin: 10px 0 20px;

                li {
                    margin: 4px 0;

                    a {
                        text-decoration: none;
                        color: gray;

                        &:hover {
                            text-decoration: underline;
                        }
                    }
                }
            }
        }

        .right img {
            width: 30%;
            position: absolute;
            top: -80px;
            right: 250px;
            z-index: 1;
        }
    }

    .bottom {
        background-color: #303030;
        width: 100%;
        height: 90px;
        padding: 0 250px;
        position: relative;
        z-index: 2;
        @include d-flex (between);

        a {
            border: 2px solid $primary-color;
            padding: 10px;
            text-decoration: none;
            color: white;
            font-size: 12px;
            font-weight: bold;

            &:hover {
                background-color: $primary-color;
            }
        }

        .follow {
            @include d-flex (center);
            height: 100%;

            span {
                color: $primary-color;
                font-weight: bold;
                margin-right: 15px;
            }

            img {
                margin: 0 7px;
                height: 30%;
                cursor: pointer;

                &:hover {
                    filter: brightness(2);
                }
            }
        }

    }

}
</style>