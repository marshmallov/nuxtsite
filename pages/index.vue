<template>
  <div>
    <Navbar/>
    <MainContent/>
    <Footer/>
  </div>
  
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'
import MainContent from '~/components/MainContent.vue';

export default {
  name: 'IndexPage',
  components: {
    Navbar,
    Footer,
    MainContent
  }
}
</script>
<style >
html,
body {
  height: 100%;
  margin: 0;
  font-family: 'Bold',
}
</style>
  