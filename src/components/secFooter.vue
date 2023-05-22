<script>
export default {
  data() {
    return {
      dcLogoBig: "dc-logo-bg.png",
    };
  },

  methods: {
    getImagePath(img) {
      return new URL(`../assets/img/${img}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="bgcontainer">
    <div class="container">
      <ul class="footer-bg">
        <li class="footer-menu">
          DC COMICS
          <ul>
            <li><a href="#"> Character</a></li>
            <li><a href="#"> Comics</a></li>
            <li><a href="#"> Movies</a></li>
            <li><a href="#"> TV</a></li>
            <li><a href="#"> Games</a></li>
            <li><a href="#"> Videos</a></li>
            <li><a href="#"> News</a></li>
          </ul>
          <ul>
            SHOP
            <li><a href="#"> Shop DC</a></li>
            <li><a href="#"></a> Shop DC Collectibles</li>
          </ul>
        </li>
        <li class="footer-menu">
          DC
          <ul>
            <li><a href="#"> Terms of Use</a></li>
            <li><a href="#"> Privacy</a></li>
            <li><a href="#"> Ad Choices</a></li>
            <li><a href="#"> Advertising</a></li>
            <li><a href="#"> Jobs</a></li>
            <li><a href="#"> Subscription</a></li>
            <li><a href="#"> Talent Workshops</a></li>
            <li><a href="#"> CPSC Certificates</a></li>
            <li><a href="#"> Ratings</a></li>
            <li><a href="#"> Shop Help</a></li>
            <li><a href="#"> Contact Us</a></li>
          </ul>
        </li>
        <li class="footer-menu">
          SITES
          <ul class="sec-footer">
            <li><a href="#"> DC</a></li>
            <li><a href="#"> MAD Magazine</a></li>
            <li><a href="#"> DC Kids</a></li>
            <li><a href="#"> DC Universe</a></li>
            <li><a href="#"> DC Power Visa</a></li>
          </ul>
        </li>
      </ul>
      <div class="img-dc">
        <img :src="getImagePath(dcLogoBig)" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
.bgcontainer {
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
}
.container {
  @include container-size;
  @include display-flex;

  .footer-bg {
    @include display-flex;
    flex: 0 0 50%;
  }

  .footer-menu {
    color: white;
    flex: 0 0 20%;
    list-style: none;
    text-decoration: none;
  }

  .sec-footer a {
    color: white;
    list-style: none;
    text-decoration: none;
  }

  .img-dc {
    flex: 0 0 50%;
    height: 100%;
    overflow: hidden;

    img {
      width: 400px;
    }
  }
}
</style>
