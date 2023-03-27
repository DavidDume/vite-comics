<script >
  import Header from './components/Header.vue'
  import Footer from './components/Footer.vue'
  import Jumbotron from './components/Jumbotron.vue'
  import Icons from './components/Icons.vue'

  export default {
    components: {
      Header,
      Footer,
      Jumbotron,
      Icons
    }
  }
</script>

<template>

  <div class="container">
    <Header></Header>
  </div>
  <div class="jumbo">
    <div class="container">
      <Jumbotron></Jumbotron>
    </div>
  </div>
  <div class="icons">
    <Icons></Icons>
  </div>

    
  

<Footer></Footer>
</template>

<style lang="scss">
@use './general.scss';
</style>
