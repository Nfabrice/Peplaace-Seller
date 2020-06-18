<template>
  <div class="home">
    <NavBar/>
    <Body />
    <SellerFooter/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/Nav/NavBar.vue'
import Body from '@/components/SellerBody/Body.vue'
import SellerFooter from '@/components/Footer/SellerFooter.vue'
import Footer from '@/components/Footer/Footer.vue'
export default {
  name: 'Home',
  components: {
    NavBar,
    Body,
    SellerFooter,
    Footer
  }
}
</script>

<style scoped>
</style>
