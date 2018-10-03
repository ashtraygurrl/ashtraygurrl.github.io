<template>
  <div class="separator">
    <span class="separator__word">
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
      default: 1,
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
  justify-content: space-between;
  align-items: center;
  align-content: center;
  padding: 16px;
  margin: 0 -12px;

  &__word {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 90px;
    font-family: 'RNS Miles';
    color: black;
    margin-left: 30%;
  }
}
</style>
