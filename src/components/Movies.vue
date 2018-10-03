<template>
  <section class="movies-section">
    <div class="container">
      <div class="columns is-multiline">
        <article class="movie-item-main">
          <div>
            <figure class="image is-3by4">
              <img class="movie-1" src="/clueless.jpg">
            </figure>
          </div>
          <div class="title-1">
            <h4>Clueless- 1995</h4>
          </div>
        </article>

         <article class="item-2">
          <div>
            <figure class="imagee is-3by4">
              <img class="movie-2" src="/robot.jpg">
            </figure>
          </div>
          <div class="title-2">
            <h4>Mr. Robot 2015-</h4>
          </div>
        </article>

        <article class="item-3">
          <div>
            <figure class="imageee is-3by4">
              <img class="movie-3" src="/gossip.jpg">
            </figure>
          </div>
          <div class="title-3">
            <h4>Gossip Girl 2007-2012</h4>
          </div>
        </article>
      </div>
        <h3 class="moviesss">FAVS MOVIES AND SERIES</h3>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import '../styles/_colors';
@import '~bulma/bulma.sass';

.movies-section{
  background-color: $white;
  color: $black;
  min-height: 650px;
  font-family: calibri;

   .image{ width: 400px;
  margin-top: 20%;
  }

  .title-1{ font-size: 25px;
  margin-left: 30%; 
  }
  
.item-2{

  .imagee{
    width: 400px;
    margin-top: 60%;
    margin-left: 20%;
    border: 20px solid $black;
    box-sizing: border-box;
  }
  .title-2{ font-size: 25px;
    margin-left: 50%; 
  }
}  
.item-3{

  .imageee{width: 400px;
    margin-top: 20%;
    margin-left: 50%;
    border: 20px solid $black;
    box-sizing: border-box;}
  .title-3{font-size: 25px;
  margin-left: 60%; }
} //item 3

.moviesss{
  font-family: 'Alesand', sans-serif;
  font-size: 90px;
  text-transform: uppercase;
  margin-top:5% ;
  margin-left: 15%;
}
} //movies section

</style>

