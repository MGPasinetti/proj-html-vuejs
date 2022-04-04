<template>
  <section class="contact-form-sec">
      <div class="container-sec">
            <h1>Latest Posts</h1>
            <small>If you are planning on developing a product landing.</small>
            <div class="posts-grid">
                <CardPost class="card-post" v-for="post in arrPosts" :key="post.srcImg" :post-data="post"/>
            </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

</style>