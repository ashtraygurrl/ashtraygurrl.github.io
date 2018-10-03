<template>
  <main>
    <AppHeader/>
    <Music text="Music" :repetitions="310"/> 
    <Bands/>
    <Series text="Movies & Series" :repetitions="1"/>
    <Movies/>
  </main>
</template>

<script>
import AppHeader from '../components/Header.vue'
import Bands from '../components/Bands.vue'
import Movies from '../components/Movies.vue'
import Music from '../components/Music.vue'
import Series from '../components/Series.vue'

export default {
  name: 'app',
  components: {
    AppHeader,
    Bands,
    Movies,  
    Music,
    Series
  }
}
</script>