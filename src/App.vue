<template>
  <div id="app">
    <the-header :nav="navItems" />
    <the-jumbo />
    <the-main />
    <select-buy-comics />
    <the-footer />
    
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import TheMain from './components/TheMain.vue'
import TheJumbo from './components/TheJumbo.vue'
import SelectBuyComics from './components/SelectBuyComics.vue'

export default {
  name: "App",
  components: {
    TheHeader,
    TheFooter,
    TheMain,
    TheJumbo,
    SelectBuyComics
  },
  data() {
    return {
      navItems: [
        'CHARACTERS',
        'COMICS',
        'MOVIES',
        'TV',
        'GAMES',
        'COLLECTIBLES',
        'VIDEOS',
        'FANS',
        'NEWS',
        'SHOP'
      ],
    }
  }
};
</script>

<style lang="scss">
@import './style/main.scss';
</style>
