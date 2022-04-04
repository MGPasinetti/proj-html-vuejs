<template>
  <header class="container-sec">
    <!-- LOGO -->
    <div class="logo">
      <img src="../assets/img/logo-2.png" alt="sofbox logo" style="height: 3rem;">
    </div>

    <!-- NAVBAR + SEARCH-i + SHOP-i + BUTTON -->
    <div>
      <NavbarHeader />
      <i class="fa-solid fa-magnifying-glass"></i>
      <i class="fa-solid fa-cart-shopping"></i> <!-- + number items rounded -->
      <button>Get Started</button>
    </div>
  </header>
</template>

<script>
import NavbarHeader from './NavbarHeader.vue';

export default {
  name: 'HeaderSb',
  components: {
    NavbarHeader,
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

header {
  display: flex;
  justify-content: space-between;
  align-items: center;

  div:last-child {
    display: flex;
    justify-content: space-between;
  }
}
</style>