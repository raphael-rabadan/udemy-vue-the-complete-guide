<template>
  <div class="container">
    <Header />
    <hr />
    <Content />
    <hr />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import Content from "./components/Content.vue"
import Footer from "./components/Footer.vue"
export default {
  components: {
    Header,
    Content,
    Footer
  }
}
</script>

<style></style>
