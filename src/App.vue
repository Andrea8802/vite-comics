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

<style lang="scss">
@use "./assets/styles/general.scss" as *;
</style>
