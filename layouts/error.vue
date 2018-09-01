<template>
  <div class="container">
    <h1 v-if="error.statusCode === 404">Seite nicht gefunden (404)</h1>
    <h1 v-else>Es ist ein Fehler aufgetreten ( {{ error.statusCode }} )</h1>
    <hr>
    <p>Schau doch einfach bei meinen <nuxt-link to="/offer/">Angeboten</nuxt-link> vorbei</p>
    <p>oder nimm direkt mit mir <nuxt-link to="/contact/">Kontakt</nuxt-link> auf.</p>
    <hr>
    <p>Vielleicht wolltest du auch meinen privaten Blog lesen? Der ist jetzt auf <a href="https://wust.me">https://wust.me</a>.</p>
  </div>
</template>

<script>
export default {
  head: {
    title: "Fehlerseite"
  },
  props: ["error"],
  layout: "default" // you can set a custom layout for the error page
};
</script>