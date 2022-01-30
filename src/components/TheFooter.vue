<template>
  <footer>
    <div class="upper">
      <div class="full-width">
        <div class="container">
          <div class="row">
            <div class="lists-container">
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
export default {
  
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.upper {
  .full-width {
    background: url('../assets/footer-bg.jpg') center;
    background-size: cover;
    height: 300px;

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

      .list{
        h2 {
          margin-bottom: .5em;
        }
        ul {
          list-style: none;
          li {
            font-size: 14px;
            margin-top: .2em;
          }
        }
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

</style>