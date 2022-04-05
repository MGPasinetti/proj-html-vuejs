<template>
  <div class="card">
      <!-- COL-1 -->
      <img src="../assets/img/24.png" alt="">
      
      <!-- COL-2 -->
      <div>
          <h3>Online Marketing</h3>
          <small>It is a long established fact that a reader will be distracted.</small>
          <ul>
              <li><i class="fas fa-check"></i>SEO</li>
              <li><i class="fas fa-check"></i>SEM</li>
              <li><i class="fas fa-check"></i>Website Strategy</li>
              <li><i class="fas fa-check"></i>Social management</li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
 name: 'CardMarketing',
}
</script>

<style lang="scss" scoped>
@import "../assets/styles/style.scss";

.card {
    display: flex;

    img {
        width: 50px;
        height: 57px;
        margin-right: 1rem;
    }

    ul {
        margin-top: 2rem;

        li {
            font-size: 12px;
            font-weight: 400;
            margin-bottom: .7rem;
        }
    }
}
</style>