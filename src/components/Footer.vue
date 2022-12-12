<script>
export default {
    name: "Footer",
    data() {
        return {
            logoImageBg: "./src/assets/img/dc-logo-bg.png"
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
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                    </ul>
                </div>

                <div class="list">
                    DC
                    <ul>
                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>

                        <li>
                            DDD
                        </li>
                    </ul>
                </div>

                <div class="list">
                    SITES
                    <ul>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                    </ul>
                </div>

                <!-- A CAPO -->
                <div class="list">
                    SHOP
                    <ul>
                        <li>
                            CCC
                        </li>
                        <li>
                            CCC
                        </li>
                    </ul>
                </div>
            </div>

            <div class="right">
                <img :src="logoImageBg" alt="">
            </div>
        </section>

        <section class="bottom">

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
    padding: 30px 250px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.left {
    display: flex;
    flex-wrap: wrap;
    width: 25%;
    gap: 30px;
    color: white
}

.right img {
    width: 30%;
    position: absolute;
    top: -80px;
    right: 280px;
    z-index: 1;
}

.bottom {
    background-color: #303030;
    width: 100%;
    height: 120px;
    position: relative;
    z-index: 2;

}
</style>