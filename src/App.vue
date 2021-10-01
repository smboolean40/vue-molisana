<template>
  <div id="app">
    <Header/>
    <Hero :bgImage="require('./assets/images/bg-prods.jpg')" title="Titolo Hero"/>
    <Hero :bgImage="require('./assets/images/footer.jpg')" title="Titolo Hero Footer"/>
    <main>
      <Products/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Products from './components/Products.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Products,
    Footer,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/common";

</style>
