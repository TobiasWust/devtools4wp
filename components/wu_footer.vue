<template>
  <div :class="{ 'indexnav' : (page === 'index') }">
    <nuxt-link exact to="/privacy/">Datenschutz</nuxt-link> |
    <nuxt-link exact to="/legal/">AGB</nuxt-link> |
    <nuxt-link exact to="/imprint/">Impressum</nuxt-link>
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
  background-color: #3dba6a;
  color: white;
  transition: all 1s ease;
}
</style>