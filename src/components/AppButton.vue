<template>
  <div>
    <slot></slot>
  </div>
</template>

<script>
export default {
  
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

div {
  background-color: $dc-blue;
  display: inline-block;
  padding: .5em 1em;
  font-weight: bold;
  font-size: 22px;
  color: #fff;      
}
</style>
