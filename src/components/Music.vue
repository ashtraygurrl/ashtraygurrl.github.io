<template>
  <div class="separator">
    <span class="separator__word" v-for="n in repetitions" :key="n">
      {{text}}
    </span>
  </div>
</template>
<script>
export default {
  props: {
    text: {
      type: String,
      default: 'Hola',
      required: false
    },
    repetitions: {
      type: Number,
      default: 315,
      required: false
    }
  }
}
</script>
<style lang="scss" scoped>
@import '../styles/_colors';
@import '../styles/_icons';
@import '~bulma/bulma.sass';

.separator{
  background-color: yellow;
  display: flex;
  flex-wrap: wrap;
  //justify-content: space-between;
  align-items: center;
  align-content: center;
  padding: 16px;
  margin: 3 -12px;

  &__word {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 18px;
    font-family: 'RNS Miles';
    line-height: 1.8;
    color: black;
    margin-left: 0px;
  }
}
</style>
