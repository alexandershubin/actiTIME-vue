<template>
<main class="main">
  <section class="features">
    <h2 class="visually-hidden">Features</h2>
    <h2 class="features__header">Features</h2>
    <p class="features__description">Some of the features and advantages that we provide for those of
      you who store data in this Data Warehouse.</p>
  <div class='slider'>
    <div class="wrapper">
    <Slider-item
      v-for="item in slider_data"
      :key="item.id"
      :item_data="data"
    />
  </div>
  </div>
   </section>
  </main>
</template>

<script>
  import SliderItem from './Slider-item.vue'
  export default {
    name: "slider",
    components: {
      SliderItem
    },
    props: {
      slider_data: {
        type: Array,
        default: () => []
      }
    },
    data() {
      return {}
    },
    computed: {

    }
  }
</script>

