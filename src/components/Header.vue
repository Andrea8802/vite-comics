<script>

export default {
    name: "Header",
    data() {
        return {
            logoImage: "./src/assets/img/dc-logo.png"
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
    gap: 30px;
}
</style>
