<template>
  <div>
    <Block></Block>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Block from './components/_base/Block'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    Block
  }
}
</script>

<style lang="scss">
  #app {
    font-family: $f-family;
    font-size: $f-size;
    color: $c-second;

    min-height: 100vh;
    background-color: $c-base-c;
  }
  * {
    transition: .25s ease;
  }


  .main {
    padding: 1rem 0;
    display: flex;
    gap: 1.5rem;

    &__content {
      display: flex;
      flex-direction: column;
      gap: .5rem;
    }
  }


  .icon {
    width:  1em;
    height: 1em;
  }


</style>
