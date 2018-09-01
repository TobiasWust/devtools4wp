<template>
<div>
  <div id="eyecatcher">
    <h1>Devtools4WP</h1>
    <span class="undertext">Nutze ganz einfach die Chrome Devtools für Wordpress!</span>
    <wu_button/>
  </div>  
</div>
</template>

<script>
import wu_button from "~/components/wu_button.vue";

export default {
  data() {
    return {};
  },
  components: {
    wu_button
  }
};
</script>

<style scoped>
h1 {
  font-size: 10vw;
  animation: rotate 90s 0s infinite alternate;
  color: #ffcc00;
  text-shadow: 1px 1px 2px #111;
}

.undertext {
  color: #111;
  font-weight: bold;
  font-size: 2em;
  text-shadow: 1px 1px 2px #ffcc00;
}

@keyframes rotate {
  from {
    transform: rotateY(50deg) rotateZ(-5deg);
  }
  to {
    transform: rotateY(-50deg) rotateZ(+5deg);
  }
}

#eyecatcher {
  padding-top: 10vh;
  text-align: center;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
</style>
