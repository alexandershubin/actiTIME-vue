<template>
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
</template>

<script>
export default {
  name: 'slider-item',
  props: {
    item_data: {
      type: Object,
      default: () => {}
    }
  },
  data() {
    return {}
  },
  computed: {}
}
</script>