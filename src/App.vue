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

<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}

ul {
  list-style: none;
}
</style>
