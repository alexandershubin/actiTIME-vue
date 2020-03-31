<template>
  <div id="app">
    <Header/>
    <Slider/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Slider from './components/Slider.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Slider,
    Footer
  }
}
</script>
