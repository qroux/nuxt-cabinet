<template>
  <div>
    <Navbar />

    <nuxt key />

    <Footer />
  </div>
</template>

<script>
import Navbar from '../components/navbar/Navbar'
import Footer from '../components/footer/Footer'
export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style lang="scss">
$fond-light: #f2f2f2;

html {
  min-height: 100vh;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: inherit;
}
body {
  font-family: 'Montserrat', sans-serif;
  position: relative;
  margin: 0;
  min-height: 100vh;
  background-color: $fond-light !important;
}
</style>
