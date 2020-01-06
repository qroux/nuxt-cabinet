<template>
  <div>
    <Navbar />
    <transition name="slide" mode="out-in">
      <nuxt />
    </transition>
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

/*custom transitions*/
.slide-enter-active {
  animation: slide-in 500ms ease-out forwards;
}
/*.slide-leave-active {
  animation: slide-out 10000ms ease-in forwards;
}*/
@keyframes slide-in {
  from {
    transform: translateY(-10px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}
/*@keyframes slide-out {
  from {
    transform: translateX(0);
    opacity: 1;
  }
  to {
    transform: translateX(-10px);
    opacity: 0;
  }
}*/
</style>
