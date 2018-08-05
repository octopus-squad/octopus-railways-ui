<template>
  <div id="app">
    <app-hero></app-hero>    
  </div>
</template>

<script>
import Hero from './components/Hero'
export default {
  name: 'app',
  components: {
    appHero: Hero
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
@import "~bulma";
@font-face {
  font-family: 'C64';
  src: url('./assets/C64_Pro-STYLE.woff') format('woff');
};
body {
  font-family: 'C64';
}
</style>

