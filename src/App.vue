<template>
  <div id="app">
    <the-header></the-header>
    <the-jumbo/>
    <the-main></the-main>
    <the-footer></the-footer>
    
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import TheMain from './components/TheMain.vue'
import TheJumbo from './components/TheJumbo.vue'

export default {
  name: "App",
  components: {
    TheHeader,
    TheFooter,
    TheMain,
    TheJumbo
  },
};
</script>

<style lang="scss">
@import './style/main.scss';
</style>
