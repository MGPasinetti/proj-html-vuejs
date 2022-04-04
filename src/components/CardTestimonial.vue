<template>
  <div class="card">
    <img :src="cardData.srcImg" :alt="cardData.name">
    <span>{{ cardData.name }} - <small>{{ cardData.role }}</small></span>
    <p>{{ cardData.msg }}</p>
  </div>
</template>

<script>
export default {
  name: 'CardTestimonial',
  props: {
      cardData: Object,
  },
}
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>