<script>
export default {
    name: "BlueBar",
    data() {
        return {

        }
    }
}
</script>

<template>
    <section>
        <ul>
            <li>
                BBB
            </li>

            <li>
                BBB
            </li>

            <li>
                BBB
            </li>

            <li>
                BBB
            </li>

            <li>
                BBB
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
    padding: 0 150px;
    position: relative;
    z-index: 2;
}

ul {
    height: 100%;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
</style>