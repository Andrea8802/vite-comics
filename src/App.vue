<script>
import Header from './components/Header.vue'

export default {
  name: "app",
  components: {
    Header
  }
}
</script>

<template>
  <Header />
</template>

<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
