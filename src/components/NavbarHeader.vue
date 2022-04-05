<template>
  <nav>
      <ul>
          <li v-for="(link, index) in links" :key="index" @click="setActiveLink(index)" :class="{active: index == activeLink }"><a href="#">{{ link }}</a></li>
      </ul>
  </nav>
</template>

<script>
export default {
    name: 'NavbarHeader',
    data() {
        return {
            activeLink: 0,
            links: [
                'Home',
                'About us',
                'Feature',
                'Testimonials',
                'Contact US'
            ]
        };
    },
    methods: {
        setActiveLink (index) {
            this.activeLink = index;
        },
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

nav {
    line-height: 35.9px;

    ul {
        @include flex-layout;
        gap: 1.5rem;
    }
}
</style>