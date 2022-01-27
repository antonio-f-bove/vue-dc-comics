<template>
<div class="full-width">
  <div class="container">
    <ul>
      <li>
        <img src="../assets/buy-comics-digital-comics.png" alt="">
        <span>DIGITAL COMICS</span>
      </li>
      <li>
        <img src="../assets/buy-comics-merchandise.png" alt="">
        <span>MERCHANDISE</span>
      </li>
      <li>
        <img src="../assets/buy-comics-subscriptions.png" alt="">
        <span>SUBSCRIPTIONS</span>
      </li>
      <li>
        <img src="../assets/buy-comics-shop-locator.png" alt="">
        <span>SHOP LOCATOR</span>
      </li>
      <li>
        <img src="../assets/buy-dc-power-visa.svg" alt="">
        <span>DC POWER VISA</span>
      </li>
    </ul>
  </div>
</div>
</template>

<script>
export default {
  
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.full-width {
  background-color: $dc-blue;
}

.container {
  width: $container-width;
  height: 150px;
  margin: 0 auto;
}

ul {
  list-style: none;
  height: 100%;
  display: flex;
  justify-content: space-evenly;

  li {
    display: flex;
    align-items: center;

    img {
      height: 40%;
    }
    span {
      color: #fff;
      margin-left: 10px;
    }
    &:last-child {
      img {
        height: 30%;
      }
    }
  }
}
</style>