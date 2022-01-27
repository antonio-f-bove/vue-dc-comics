<template>
  <footer>
    <div class="upper">
      <div class="full-width">
        <div class="container">
          <div class="list">
            <h2>DC COMICS</h2>
            <ul>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
            </ul>
          </div>

          <div class="list">
            <h2>SHOP</h2>
            <ul>
              <li>lorem</li>
              <li>lorem</li>
            </ul>
          </div>

          <div class="list">
            <h2>DC</h2>
            <ul>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
            </ul>
          </div>

          <div class="list">
            <h2>SITES</h2>
            <ul>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
              <li>lorem</li>
            </ul>
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
export default {
  
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.container {
  width: $container-width;
  margin: 0 auto;
}

.upper {
  .full-width {
    background: url('../assets/footer-bg.jpg') center;
    background-size: cover;
    height: 400px;

    color: #fff;
  }

  ul {
    list-style: none;

    
  }
}

</style>