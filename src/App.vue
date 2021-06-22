<template>
  <div id="app">
    <Header
    :links="mainLinks" />


    <Footer
    :explore="exploreLinks"
    :informations="informationLinks"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer
  },
  data() {
    return {
      mainLinks: ["Home","Pages","Courses","Features","Blog","Shop"],
      exploreLinks: ["Start here","Blog", "About us", "Success story", "Courses", "Contact us"],
      informationLinks: ["Membership","Purchase guide","Privacy policy","Terms of service"]
    }
  }
}
</script>

<style lang="scss">
  * {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
  }
</style>
