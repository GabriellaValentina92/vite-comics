<script></script>

<template>
  <div class="bg-color">
    <div>
      <button>SIGN-UP NOW!</button>
    </div>
    <div class="icons">
      <h2>FOLLOW US</h2>
      <img src="../../img/footer-facebook.png" alt="" />
      <img src="../../img/footer-periscope.png" alt="" />
      <img src="../../img/footer-pinterest.png" alt="" />
      <img src="../../img/footer-twitter.png" alt="" />
      <img src="../../img/footer-youtube.png" alt="" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.bg-color {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100px;
  background-color: black;
  padding: 0.5rem;

  .icons {
    display: flex;
    align-items: center;
  }
  .icons h2 {
    color: rgb(17, 138, 237);
    font-size: 1.3rem;
    padding: 0.5rem;
  }

  .icons img {
    padding: 0.5rem;
  }
}
</style>
