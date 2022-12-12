<script>
import Header from './components/Header.vue'
import BlueBar from './components/BlueBar.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'

export default {
  name: "app",
  components: {
    Header,
    Content,
    BlueBar,
    Footer
  }
}
</script>

<template>
  <Header />
  <main>
    <Content />
    <BlueBar />
  </main>
  <Footer />
</template>

<style lang="scss">
@use "./assets/styles/general.scss" as *;
@use "./assets/styles/partials/mixins.scss" as *;
</style>
