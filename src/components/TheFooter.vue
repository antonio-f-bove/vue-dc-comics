<template>
  <footer>
    <div class="upper">
      <div class="full-width">
        <div class="container">
          <div class="row">
            <div class="lists-container">
              <list-footer v-for="(item, i) in items" 
              :key="i" 
              :list="item" 
              class="list-footer"
              />
            </div>

            <div class="logo-container">
              <img src="../assets/dc-logo-bg.png">
            </div>
          </div>
        </div>
      </div>
    </div>      

    <div class="lower">
      <div class="full-width">
        <div class="container">

        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import ListFooter from './ListFooter.vue'

export default {
  components: {
    ListFooter
  },
  props: {
    items: Array
  }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.upper {
  .full-width {
    background: url('../assets/footer-bg.jpg') center;
    background-size: cover;
    height: 360px;

    color: #fff;
  }

  .container {
    width: $container-width;
    height: 100%;
    margin: 0 auto;
  }

  .row {
    height: 100%;
    display: flex;

    .lists-container {
      width: 50%;
      padding: 36px 0;
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
      align-content: flex-start;

      .list-footer {
        margin-right: 36px;
      }
    }

    .logo-container {
      width: 50%;
      overflow: hidden;
      img {
        height: 150%;
        transform: translateY(-15%);
      }
    }
  }
}

.lower {
  .full-width {
    height: 100px;
    background-color: #333;
  }
}

</style>