<template>
  <section class="bands-section">
    <div class="container">
      <div class="columns is-multiline">
        <article class="band-item--main">
          <div class="letras-1">
            <h4 class="title-1">Essential Placebo Albums</h4>
            <ol class="list-1">
            <li>Meds</li>
            <li>Sleeping with Ghosts</li>
            <li>Black Market Music</li>
           </ol>
          </div>
          <div>
            <figure class="image is-3by4">
              <img class="band-1" src="/img/placebo.jpg" >
            </figure>
          </div>
        </article>

        <h3 class="bandsss"> FAVS BANDS AND ALBUMS </h3>

        <article class="band-item">
          <div class="letras-2">
            <h4 class="title-2">Essential Antics Tracks</h4>
            <ol class="list-2">
            <li>C´mere</li>
            <li>Public Pervert</li>
            <li>Slow Hands</li>
           </ol>
          </div>       
          <div>
            <figure class="image is-3by2">
              <img class="band-2" src="/img/antics.jpg" >
            </figure>
          </div>
        </article>
     </div>
  
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import '../styles/_colors';
@import '~bulma/bulma.sass';

.band-item--main {
  @extend .column;
  @extend .is-8;
  @extend .is-offset-1;
  font-family:calibri;
  display: flex;

  .letras-1 {
    margin-top:20%;
    margin-left: 5%;
    font-size: 25px;

  }

  .title-1 {
    font-size: 30px;
    margin-left: -25px;
  }

  .image {
    width: 450px;
    margin-left: 10%;
    
  }
}

.bands-section{
  background-color: $black;
  color: white;
  min-height: 650px;
}

.band-item {
  @extend .column;
  @extend .is-6;
  @extend .is-offset-5;
  font-family: calibri;
  
  .letras-2 {
    margin-top: 10%;
    margin-left: -30%;
    font-size: 25px;
  }

  .title-2 {
    font-family: calibri;
    font-size: 30px;
    margin-left: -25px;
  }
  .band-2{
    margin-top: -18%;
    margin-left: 10%;
  }
  
}

.bandsss{
  font-family: 'Alesand', sans-serif;
  font-size: 90px;
  text-transform: uppercase;
  margin-top:5% ;
  margin-left: 10%;
  
}

</style>
