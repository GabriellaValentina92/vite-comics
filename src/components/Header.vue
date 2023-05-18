<script></script>

<template>
  <ul class="navbar">
    <li class="logo">
      <img src="../../img/dc-logo.png" alt="" />
    </li>
    <ul class="nav-menu">
      <li>CHARACTER</li>
      <li>COMICS</li>
      <li>MOVIES</li>
      <li>TV</li>
      <li>GAMES</li>
      <li>COLLECTIBLES</li>
      <li>VIDEOS</li>
      <li>FANS</li>
      <li>NEWS</li>
      <li>SHOPS</li>
    </ul>
  </ul>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
$bg-color: white;
.navbar {
  @include display-flex;

  .logo img {
    width: 60px;
  }

  .nav-menu {
    display: flex;
  }

  .nav-menu li {
    color: black;
    font-weight: 500;
    list-style: none;
    padding: 0.5rem;
  }
}
</style>
