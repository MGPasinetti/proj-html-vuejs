<template>
  <section class="container-sec grid-cards">
    <CardMarketing />
    <CardMarketing />
    <CardMarketing />
  </section>
</template>

<script>
import CardMarketing from './CardMarketing.vue';

export default {
  name: 'GridCardsSec',
  components: {
    CardMarketing,
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.grid-cards {
  display: flex;
}
</style>