<template>
  <dir>
      <h3>{{ listData.title }}</h3>
      <ul>
        <li v-for="link in listData.arrLinks" :key="link"><a href="#">{{ link }}</a></li>
      </ul>
  </dir>
</template>

<script>
export default {
  name: 'ListFooter',
  props: {
    listData: Object,
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

</style>