<script></script>

<template>
  <ul>
    <li class="shopOnline">
      <ul class="links">
        <li>
          <img src="../../img/buy-comics-digital-comics.png" alt="" />
        </li>
        <li>DIGITAL COMICS</li>
      </ul>

      <ul class="links">
        <li>
          <img src="../../img/buy-comics-merchandise.png" alt="" />
        </li>
        <li>DC MERCHANDISE</li>
      </ul>

      <ul class="links">
        <li>
          <img src="../../img/buy-comics-subscriptions.png" alt="" />
        </li>
        <li>SUBSCRIPTION</li>
      </ul>

      <ul class="links">
        <li>
          <img src="../../img/buy-comics-shop-locator.png" alt="" />
        </li>
        <li>COMIC SHOP LOCATOR</li>
      </ul>

      <ul class="links">
        <li>
          <img src="../../img/buy-dc-power-visa.svg" alt="" />
        </li>
        <li>DC POWER VISA</li>
      </ul>
    </li>
  </ul>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
ul {
  background-color: rgb(7, 127, 246);
}

.shopOnline {
  @include merch-display-flex;
  min-height: 100px;
  .links {
    display: flex;
    list-style: none;
  }
}
.links li img {
  width: 30px;
  margin-right: 0.8rem;
}
</style>
