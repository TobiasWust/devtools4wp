<template>
  <div :class="{ 'indexnav' : (page === 'index') }">
    <nuxt-link exact to="/datenschutz/">Datenschutz</nuxt-link> |
    <!-- <nuxt-link exact to="/AGB/">AGB</nuxt-link> | -->
    <nuxt-link exact to="/impressum/">Impressum</nuxt-link>
  </div>
</template>

<script>
import { mapState } from "vuex";

export default {
  computed: mapState(["page"])
  //  :class="{ 'active' : (page === 'index') }"
};
</script>

<style scoped>
div {
  margin-top: 4em;
}
.nuxt-link-active {
  color: #111;
}
.indexnav {
  background: none;
  transition: all 1s ease;
}
a {
  color: white;
  text-decoration: none;
}
div {
  text-align: center;
  background-color: #ffcc00;
  color: white;
  transition: all 1s ease;
}
</style>