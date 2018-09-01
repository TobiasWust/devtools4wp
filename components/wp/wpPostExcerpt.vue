<template>
  <div>
      <h2><nuxt-link :to="post.slug + '/'">{{ post.title.rendered }}</nuxt-link></h2>
      <p>{{ post.slug }}</p>
      <div v-html="post.excerpt.rendered"></div>      
  </div>
</template>

<script>
export default {
  props: ["post"]
};
</script>

<style scoped>
</style>