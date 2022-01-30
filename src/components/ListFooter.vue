<template>
  <div>
    <h2>{{ list.label }}</h2>
    <ul>
      <li v-for="(item, i) in list.items" :key="i">{{ item }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    list: Object
  }
}
</script>

<style lang="scss" scoped>
div {
  h2 {
    margin-bottom: .5em;
  }
  ul {
    list-style: none;
    li {
      font-size: 14px;
      margin-top: .2em;
      color: #aaa;
    }
  }
}
</style>