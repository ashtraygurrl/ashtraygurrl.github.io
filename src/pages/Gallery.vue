<template>
  <header class="gallery-header">
    <section class="gallery-header__content">
      <div class="container">
         <nav class="site-nav__back">
             <router-link class="site-nav__link active" to="/">
      <span class=" column is-1 icon-eye"></span>
     </router-link>
         </nav>
          
        <div class="columns is-multiline">
           
          <article class="column is-4 i1">
            <div>
              <figure class="image is-square">
                <img src="/palm.jpg" >
              </figure>
            </div>
          </article>
          <article class="column is-4 i2">
            <div>
              <figure class="image is-square">
                <img src="/light.jpg" >
              </figure>
            </div>
          </article>
          <article class="column is-4 i3">
            <div>
              <figure class="image is-square">
                <img src="/olaa2.jpg" >
              </figure>
            </div>
          </article>
           <h1 class="title">GALLERY</h1>
        </div>
      </div>
    </section>
  </header>
</template>

<style lang="scss" scoped>
@import '../styles/_colors';
@import '../styles/_icons';
@import '~bulma/bulma.sass';

.gallery-header {
  @extend .hero;
  @extend .is-fullheight;
  background-color: $black;
  color: white;

  &__content { 
    @extend .hero-body;
    margin-top: -150px;
  }
}//galleryheader

.i1 {
  position: relative;
  margin-left: 16.67%;
}

.i2 {
  background-color: $black;
  border: 2px solid $white;
  box-sizing: border-box;
  position: relative;
  margin-left: -8.333%;
  transform: translateY(80%);
}

.i3 {
  background-color: $black;
  border: 2px solid $yellow;
  box-sizing: border-box;
  position: relative;
  margin-left: -13.333%;
}

.title {
  font-family: 'Alesand', sans-serif;
  font-size: 120px;
  text-transform: uppercase;
  letter-spacing: 10px;
  color:white;
  margin-top: 10%;
}

.icon-eye{
color: $white;
font-size: 100px;
margin-top: 3%

}

</style>
