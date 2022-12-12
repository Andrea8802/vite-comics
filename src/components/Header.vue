<script>

export default {
    name: "header",
    data() {
        return {
            logoImage: "src/assets/img/dc-logo.png"
        }
    }
}
</script>

<template>

    <header>
        <img :src="logoImage" alt="">
        <ul>
            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>

            <li>
                AAA
            </li>
        </ul>
    </header>


</template>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    /* DEBUG */
    background-color: red;
    height: 100px;
    width: 100%;
    padding: 0 260px;
}

header img {
    height: 60%;
}

header ul {
    display: flex;
    justify-content: space-evenly;
    align-self: center;
    gap: 30px;
    list-style: none;
}
</style>
