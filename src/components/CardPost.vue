<template>
  <div class="post">
      <img :src="postData.srcImg" :alt="postData.title">
      <span>{{ postData.date }}</span>
      <h5>{{ postData.title }}</h5>
      <p>{{ postData.text }}</p>
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
    }
}
</style>