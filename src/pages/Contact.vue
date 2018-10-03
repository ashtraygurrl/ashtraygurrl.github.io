<template>
  <header class="contact-header">
    <div class="bk">
      <lines/>
    </div>
    <Nav class="contact-header__nav"/>
    <section class="contact-header__content">
      <div class="container">
         <nav class="site-nav__back">
             <router-link class="site-nav__link active" to="/">
               <span class=" column is-1 icon-eye"></span>
              </router-link>
         </nav>
        <div class="columns">
          <article class="column is-9 hero-title">
            <h1 class="title"> CONTACT</h1>
          </article>
          <article class="column is-9 hero-info">
            <h3 class="info">guadaherr.00@gmail.com
              <br>
              5598-6250
            </h3>
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

.contact-header{
  @extend .hero;
  @extend .is-fullheight;
  background-color: $white;
  color: black;
  position: relative;

   &__content { 
    @extend .hero-body;
    margin-top: -150px;
    box-sizing: border-box;
    overflow: hidden;
  }
  .bk {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
  }

}//contactheader

.title{
  font-family: 'Alesand', sans-serif;
  font-size: 200px;
  text-transform: uppercase;
  letter-spacing: 10px;
  color:black;
  margin-top: 10%;
}

.info{
  @extend .is-offset-4;
  font-family: 'RNS Miles', sans-serif;
  font-size: 70px;
  color: black;
  margin-left: -60%;
  margin-top: 40%;
}

.icon-eye{
color: $black;
font-size: 100px;
margin-top: 2%
}

</style>
<script>
import Lines from '../components/background/Lines2'

export default {
  components: {
    Lines
  }
}
</script>



