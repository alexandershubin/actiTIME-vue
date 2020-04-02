<template>
<main class="main">
 <section class="features">
    <h2 class="visually-hidden">Features</h2>
    <h2 class="features__header">Features</h2>
    <p class="features__description">Some of the features and advantages that we provide for those of
      you who store data in this Data Warehouse.</p>
  <div class="slider">
    <carousel :responsive="{0:{items:1,nav:false},1200:{items:2,nav:false}}" :margin='10'>
      <div class="slider__item">
        <h3 class="slider__header">First Feature</h3>
        <p class="slider__description">Little Red Cap opened her eyes and when she saw the
          sunbeams dancing to and fro through the trees and how
          the ground was covered with beautiful flowers.</p>

        <a class="slider__more" href="">Learn more
          <svg width="22" height="16" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M15 15L21 8L15 1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round"
                  stroke-linejoin="round"/>
            <path d="M21 8H1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </a>
      </div>
      <div class="slider__item">
        <h3 class="slider__header">Second Feature</h3>
        <p class="slider__description">Each time she picked one she thought that she could
          see an even more beautiful one a little way off, and
          she ran after it, going further and further into the woods.</p>
        <a class="slider__more" href="">Learn more
          <svg width="22" height="16" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M15 15L21 8L15 1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round"
                  stroke-linejoin="round"/>
            <path d="M21 8H1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </a>
      </div>
      <div class="slider__item">
        <h3 class="slider__header">Third Feature</h3>
        <p class="slider__description">The wolf pressed the latch, and the door opened.
          He stepped inside, went straight to the grandmother's bed,
          and ate her up.</p>
        <a class="slider__more" href="">Learn more
          <svg width="22" height="16" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M15 15L21 8L15 1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round"
                  stroke-linejoin="round"/>
            <path d="M21 8H1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </a>
      </div>
      <div class="slider__item slider__item--new">
        <h3 class="slider__header">Fourth Feature</h3>
        <p class="slider__description">Little Red Cap had run after the flowers. After
          she had gathered so many that she could not carry any more,
          she remembered her grandmother.</p>
        <a class="slider__more" href="">Learn more
          <svg width="22" height="16" viewBox="0 0 22 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M15 15L21 8L15 1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round"
                  stroke-linejoin="round"/>
            <path d="M21 8H1" stroke="#9C69E2" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </a>
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
  };
</script>

