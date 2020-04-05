<template>
  <header class="header">
  <div class="header__container">
    <div class="header__body">
      <a href="logo" class="header__logo"><span class="visually-hidden">logo</span></a>

      <div class="header__burger" @click="click" v-bind:class="{ active: showMenu }">
        <span></span>
      </div>

      <nav class="header__menu" v-bind:class="{ active: showMenu }">
        <ul class="header__list">
          <li class="header__item">
            <a href="about.html" class="header__link">About</a>
          </li>
          <li class="header__item header__item--arrow" @click="open">
            <a href="" class="header__link">Help</a>
            <div class="arrow" v-bind:class="{ active: showSubMenu }">
              <span class="visually-hidden">открыть</span>
              <svg class="arrow__small" width="10" height="6" viewBox="0 0 10 6" fill="#212353"
                   xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd" clip-rule="evenodd"
                      d="M5.70633 2.79356C5.31582 3.18404 4.6827 3.18404 4.29219 2.79356L1.87467 0.376274C1.52957 0.0312008 0.970075 0.0312017 0.62497 0.376275C0.279818 0.721394 0.279818 1.28098 0.62497 1.6261L4.37443 5.37521C4.71954 5.72028 5.27903 5.72028 5.62414 5.37521L6.24909 4.75031C6.2491 4.7503 6.2491 4.75029 6.24909 4.75028C6.24909 4.75028 6.24909 4.75026 6.24909 4.75026L9.37503 1.62461C9.72018 1.2795 9.72018 0.719912 9.37503 0.374793C9.02992 0.0297193 8.47043 0.0297198 8.12533 0.374793L5.70633 2.79356Z"
                      fill="#212353"/>
              </svg>
            </div>
            <ul class="sub-menu" v-bind:class="{ active: showSubMenu }">
              <li class="sub-menu__item" v-for="subLink in subLinks" :key="subLink">
                <a class="sub-menu__link" href="#User">{{subLink.linkSubMenu}}</a>
              </li>
            </ul>
          </li>
          <li class="header__item"><a href="" class="header__link">Features</a></li>
        </ul>
        <button type="button" class="header__button button">Sign Up</button>
      </nav>
    </div>
  </div>
</header>
</template>

<script>
  export default {
    data() {
      return {
        showMenu:false,
        showSubMenu:false,

        subLinks: [
          {linkSubMenu: 'User Guide'},
          {linkSubMenu: 'Contact Support'},
        ],

      };
    },
    methods: {
      click () {
        this.showMenu ? this.showMenu = false : this.showMenu = true
      },
      open () {
        this.showSubMenu ? this.showSubMenu = false : this.showSubMenu = true
      }
    }
  }
</script>

