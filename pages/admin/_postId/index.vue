<template>
  <div class="admin-post-page">
    <section class="update-form">
      <admin-post-form :post="loadedPost"/>
    </section>
  </div>
</template>

<script>
import adminPostForm from '@/components/Admin/AdminPostForm'
export default {
  layout: 'admin',
  components: {
    adminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: 'Milan',
        title: 'My awesome post',
        content: 'Super amazing, thanks for that!',
        thumbnail: 'https://yw553ftvhw1iqegz29fycoyw-wpengine.netdna-ssl.com/wp-content/uploads/2017/09/technology-16-9.jpg'
      }
    }
  }
}
</script>
<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
