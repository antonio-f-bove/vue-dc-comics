<template>
  <main>
    <div class="container">
      <div class="card">
        <div class="wrapper">
          <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX">
        </div>
        <p>Lorem, ipsum dolor.</p>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  props: {
    cards: Array
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

    .card {
      width: calc(100% / 6 - 6 * 12px);
      padding: 12px 6px;

      .wrapper {
        width: 192px;
        height: 192px;

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
        width: fit-content;
      }
    }
  }
}
</style>