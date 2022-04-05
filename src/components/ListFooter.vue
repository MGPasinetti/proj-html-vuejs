<template>
  <div class="list">
    <h5>{{ listData.title }}</h5>
    <ul>
      <li v-for="link in listData.arrLinks" :key="link"><a href="#">{{ link }}</a></li>
    </ul>
  </div>
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

.list {

  ul {
    @include col-layout($direction: column, $align: flex-start);
    gap: 1rem;

    li {
      line-height: 1.2;
      font-size: 12px;
      border-bottom: 1px solid transparent;

      a {
        color: $txt_color_grey;
      }

      &:hover {
        border-bottom: 1px solid $border_color_blue;
        
        & a {
          color: $txt_color_blue;
        }
      }
    }
  }
}
</style>