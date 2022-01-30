<template>
  <main>
    <div class="container">
      <app-button id="current">CURRENT SERIES</app-button>

      <div class="row">
        <div v-for="(card, index) in cards" :key="index" class="card">
          <div class="wrapper">
            <img :src="card.thumb">
          </div>
          <p>{{ card.series.toUpperCase() }}</p>
        </div>
      </div>

      <div class="row">
        <app-button id="load">LOAD MORE</app-button>
      </div>
    </div>
  </main>
</template>

<script>
import AppButton from './AppButton.vue'

export default {
  props: {
    cards: Array
  },
  components: {
    AppButton
  }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

main {
  background: #333;

  .container {
    width: $container-width;
    margin: 0 auto;
    padding: 24px 0 12px;
    position: relative;

    .row {
      display: flex;
      flex-wrap: wrap;
  
      .card {
        width: calc(100% / 6);
        padding: 24px 10px;
  
        .wrapper {
          width: 180px;
          height: 180px;
          margin-bottom: 12px;
  
          img {
            height: 100%;
            width: 100%;
            object-fit: cover;
            object-position: top;
          }
        }
  
        p {
          color: #fff;
          font-size: 14px;
          font-weight: bold;
        }
      }
    }

    #current {
      position: absolute;
      top: 0;
      transform: translateY(-50%);
    }

    #load {
      font-size: 12px;
      padding: .75em 4em;
      margin: 0 auto;
    }
  }
}
</style>