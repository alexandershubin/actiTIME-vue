<template>
  <div id="app">
    <Header/>
    <Slider
      :slider_data="sliderItems"
      />
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
    Footer,
    Slider
  },
  data() {
    return {
      sliderItems: [
        { id: 1, name: 'img1', img: 'logo.png' },
        { id: 1, name: 'img1', img: 'logo.png' },
        { id: 1, name: 'img1', img: 'logo.png' },
        { id: 1, name: 'img1', img: 'logo.png' }
      ]
    }
  }
}
</script>
