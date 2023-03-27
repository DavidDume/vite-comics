<script >
  import Header from './components/Header.vue'
  import Footer from './components/Footer.vue'

  export default {
    components: {
      Header,
      Footer
    }
  }
</script>

<template>

  <div class="container">
    <Header></Header>
  </div>

<Footer></Footer>
</template>

<style lang="scss">
@use './general.scss';
</style>
