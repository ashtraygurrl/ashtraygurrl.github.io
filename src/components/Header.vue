<template>
  <header class="home-header">
    <div class="home-header__background">
      <lines/>
    </div>
    <Nav class="home-header__nav"/>
    <section class="home-header__content">
      <div class="container">
        <div class="columns">
          <article class="column is-9 hero-title">
            <h1 class="title name"> Guadalupe</h1>
          </article>
          <article class="column is-6 image">
            <img class="title image" src="./rat.jpg" >
          </article>
        </div>
      </div>
    </section>
  </header>
</template>

<style lang="scss" scoped>
@import '../styles/_colors';
@import '../styles/_icons';
@import '~bulma/bulma.sass';

.home-header {
  @extend .hero;
  @extend .is-fullheight;
  position: relative;

  &__nav {
    @extend .hero-head;
  }

  &__content {
    @extend .hero-body;
  }

  &__background {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
  }

  .columns {
    align-items: flex-end;
  }
}

.image {
  position: relative;
  z-index: -1;
  margin-left: calc(-16.667%  - 16px);
}


.hero-title {
  margin-bottom: 10%;
}

.name {
  font-family: 'RNS Miles', sans-serif;
  font-size: 120px;
  text-transform: uppercase;
  letter-spacing: 24px;
}
</style>

<script>
import Nav from './Nav.vue'
import Lines from './background/Lines'
export default {
  components: {
    Lines,
    Nav
  }
}
</script>

