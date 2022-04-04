<template>
  <nav>
      <ul>
          <li v-for="link in links" :key="link"><a href="#">{{ link }}</a></li>
      </ul>
  </nav>
</template>

<script>
export default {
    name: 'NavbarHeader',
    data() {
        return {
            links: [
                'Home',
                'About us',
                'Feature',
                'Testimonials',
                'Contact US'
            ]
        };
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

ul {
  display: flex;
  justify-content: space-between;
  list-style: none;
}
</style>