<template>
<main class="main">
 <section class="features">
    <h2 class="visually-hidden">Features</h2>
    <h2 class="features__header">Features</h2>
    <p class="features__description">Some of the features and advantages that we provide for those of
      you who store data in this Data Warehouse.</p>
  <div class="slider">
    <carousel :responsive="{0:{items:1,nav:false},1200:{items:2,nav:false}}" :margin='10'>
      <div class="slider__item" v-for="slide in sliders" :key="slide">
       <h3 class="slider__header">{{slide.title}}</h3>
       <p class="slider__description">{{slide.descriptions}}</p>
        <a class="slider__more" href="">{{slide.link}}</a>
      </div>
    </carousel>
  </div>
  </section>
  </main>
</template>
<script>
  import carousel from 'vue-owl-carousel'

  export default {
    components: { carousel },
    data () {
      return {
        sliders: [
          {
            title: 'First Feature',
            descriptions: 'Little Red Cap opened her eyes and when she saw the sunbeams dancing to and fro through the trees and how the ground was covered with beautiful flowers.',
            link: 'Learn more'
          },
          {
            title: 'Second Feature',
            descriptions: 'Each time she picked one she thought that she could see an even more beautiful one a little way off, and she ran after it, going further and further into the woods.',
            link: 'Learn more'
          },
           {
            title: 'Third Feature',
            descriptions: 'The wolf pressed the latch, and the door opened. He stepped inside, went straight to the grandmother/\'s bed, and ate her up.',
            link: 'Learn more'
            },
          {
            title: 'Fourth Feature',
            descriptions: 'Little Red Cap had run after the flowers. After she had gathered so many that she could not carry any more, she remembered her grandmother.',
            link: 'Learn more'
          },
        ]
      }
    }
  };
</script>

