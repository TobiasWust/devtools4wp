<template>
  <div>
    <h1>{{ post[0].title.rendered }}</h1>
    <div v-html="post[0].content.rendered"></div>
  </div>
</template>

<script>
import axios from "axios";

export default {
/*   async asyncData({ route }) {
    let { data } = await axios.get(
      `https://blog.tobiaswust.de/wp-json/wp/v2/posts/?slug=${
        route.params.slug
      }`
    );
    console.log(
      `https://blog.tobiaswust.de/wp-json/wp/v2/posts/?slug=${
        route.params.slug
      }`
    );
    return { post: data };
  } */
};
</script>

<style scoped>
</style>

