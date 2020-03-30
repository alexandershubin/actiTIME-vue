<template>
  <footer class="page-footer">
    <div class="page-footer__wrapper container">
      <div class="page-footer__link">
        <div class="page-footer__logo">
          <a href="logo" class="logo-white"><span class="visually-hidden">logo</span></a>
        </div>
        <ul class="page-footer__list">
          <li class="page-footer__item"><a class="page-footer__url" href="">About Us</a></li>
          <li class="page-footer__item"><a class="page-footer__url" href="">Privacy Policy</a></li>
        </ul>
      </div>

      <form class="form" action="#">
        <label for="email" class="visually-hidden">Введите e-mail</label>
        <input class="form__email" type="email" placeholder="Enter your e-mail" id="email" required>
        <input class="form__button button" type="submit" value="Sign Up Now">
      </form>
    </div>
  </footer>
</template>

<script>
  export default {}
</script>

