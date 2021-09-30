<template>
  <div id="app">
    <Header/>
    <main>
      <Products/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Products from '@/components/Products.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Products,
    Footer,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/common";

</style>
