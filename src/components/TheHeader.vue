<template>
  <header>
    <div class="container">
      <div class="logo-container">
        <img src="../assets/dc-logo.png">
      </div>

      <nav>
        <ul>
          <li v-for="(item, i) in nav" :key="i">
            {{ item }}
          </li>
        </ul>
      </nav>
    </div>
  </header>  
</template>

<script>
export default {
  props: {
    nav: Array,
  }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.container {
  width: $container-width;
  margin: 0 auto;
  padding: 20px 0;
  height: 150px;

  display: flex;
  justify-content: space-between;
}

nav {
  height: 100%;

  ul {
    list-style: none;
    display: flex;
    justify-content: flex-end;
    height: 100%;

      li {
        list-style: none;
        margin: 0 14px;
        font-size: 14px;
        height: 100%;
        border-bottom: solid 5px transparent;
        
        display: flex;
        align-items: center;

        &:hover {
          border-bottom: 5px solid $dc-blue;
          color: $dc-blue;
        }
      }
  }
}
</style>