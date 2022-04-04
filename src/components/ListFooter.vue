<template>
  <dir>
      <h1>{{ listData.title }}</h1>
      <ul>
        <li v-for="link in listData.arrLinks" :key="link">{{ link }}</li>
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

<style>

</style>