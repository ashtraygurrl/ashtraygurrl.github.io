<template>
  <div class="site-nav">
    <nav class="site-nav__links">
      <div class="navbar-end">
        <router-link class="site-nav__link active" to="/">home</router-link>
        <router-link class="site-nav__link" to="/gallery"> gallery </router-link>
        <router-link class="site-nav__link" to="/contact"> contact </router-link>
      </div>
    </nav>
    <nav class="site-nav__social">
      <a href="https://www.facebook.com/synergydeath">
        <span class="icon-facebook"></span>
      </a>
      <a href="https://www.instagram.com/ashtraygurrl/">
        <span class="icon-instagram"></span>
      </a>
      <a href="https://open.spotify.com/user/adwoh5xw6tjrvdz4kmqj31wy0?si=jRqonSLMQJaGkx8A1E89OQ">
        <span class="icon-spotify"></span>
      </a>
    </nav>
  </div>    
</template>

<style lang="scss" scoped>
@import '../styles/_colors';
@import '../styles/_icons';
@import '~bulma/bulma.sass';

.site-nav {
  @extend .container;

  &__links {
    @extend .navbar;
    
    background-color: transparent;  
  }

  &__link {
    @extend .navbar-item;

    background-color: transparent;
    color: $black;
    font-family: 'RNS Miles', sans-serif;
    font-size: 50px;
    position: relative;
    text-decoration: none;
    transition: transform 150ms ease-in;

    &:hover {
      background-color: transparent !important;
      color: $black !important;
      transform: scale(1.05);
    }

    &.active:before {
      background-color: $black;
      box-sizing: border-box;
      content: '';
      display: block;
      height: 3px;
      left: 50%;
      position: absolute;
      top: 40%;
      width: 100%;
      transform: rotate(-10deg) translate(-50%, -50%);
      transform-origin: 50% 50%;
    }
  }
  
  &__social {
    display: flex;
    flex-direction: column;
    left: 0;
    position: absolute;
    top: 40px;
    font-size: 80px;
    z-index: 999;

    a {
      color: $black;
      margin-bottom: 8px;
    }
  }
}

</style>
