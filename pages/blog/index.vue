<template>
  <div>
    <h1>Blog</h1>
    <hr>
    <wpList :posts="posts" />
  </div>
</template>

<script>
import wpList from "~/components/wp/wpList.vue";
import axios from "axios";

export default {
  head: {
    title: "Blog"
  },
  components: {
    wpList
  },
  async asyncData() {
    /* let { data } = await axios.get(
      "https://blog.tobiaswust.de/wp-json/wp/v2/posts/"
    );
    return { posts: data }; */
  }
};
</script>

<style scoped>
</style>