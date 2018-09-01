<template>
  <div class="blog">
    <div v-for="post in posts" :key="post.id">
      <wpPostExcerpt :post="post" />
      <hr>
    </div>
  </div>
</template>

<script>
import wpPostExcerpt from "~/components/wp/wpPostExcerpt.vue";

export default {
  name: "wpList",
  props: ["posts"],
  components: {
    wpPostExcerpt
  }
};
</script>

<style scoped>
.blog {
  font-size: 100%;
}
</style>