<template>
  <div class="post">
      <img :src="postData.srcImg" :alt="postData.title">
      <span>{{ postData.date }}</span>
      <h1>{{ postData.title }}</h1>
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