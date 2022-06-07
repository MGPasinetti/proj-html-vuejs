<template>
  <div class="post">
      <img :src="postData.srcImg" :alt="postData.title">
      <span>{{ postData.date }}</span>
      <div class="text-post">
        <h4>{{ postData.title }}</h4>
        <p>{{ postData.text }}</p>
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardPost',
    props: {
        postData: Object,
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.post {
    padding: .5rem;
    position: relative;
    border: 1px solid $border_color_whitesmoke2; 
    border-radius: 3px;
    cursor: pointer;

    img {
        width: 100%;
    }

    span {
        background-color: white;
        padding: .5rem;
        color: grey;
        position: absolute;
        top: 1rem;
        left: 1rem;
        border-radius: .3rem;
        font-size: 12px;
    }

    .text-post {
        padding: 1rem .7rem;
    }
}
</style>