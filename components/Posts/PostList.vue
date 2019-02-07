<template>
  <section class="post-list">
      <post-preview
        id="1"
        :isAdmin="isAdmin"
        thumbnail="https://yw553ftvhw1iqegz29fycoyw-wpengine.netdna-ssl.com/wp-content/uploads/2017/09/technology-16-9.jpg"
        title="Hello There!"
        previewText="Some Text 1"
      />
      <post-preview
        id="2"
        :isAdmin="isAdmin"
        thumbnail="https://yw553ftvhw1iqegz29fycoyw-wpengine.netdna-ssl.com/wp-content/uploads/2017/09/technology-16-9.jpg"
        title="Hello There!"
        previewText="Some Text 2"
      />
      <post-preview
        id="3"
        :isAdmin="isAdmin"
        thumbnail="https://yw553ftvhw1iqegz29fycoyw-wpengine.netdna-ssl.com/wp-content/uploads/2017/09/technology-16-9.jpg"
        title="Hello There!"
        previewText="Some Text 3"
      />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
