<template>
  <div id="eyecatcher">
    <h1><a href="/">Devtools4WP</a></h1>  
    <span class="undertext">Nutze ganz einfach die Chrome Devtools für Wordpress!</span>
    <wu_button/>
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
  animation: rotate 90s infinite alternate;
}
h1 a {
  font-size: 10vw;
  color: #ffcc00;
  text-shadow: 1px 1px 2px #111;
  text-decoration: none;
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
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;

  background-image: url("~/assets/img/background.png");
  /* background-image: url("https://res.cloudinary.com/tobiaswust/image/upload/c_scale,f_auto,q_auto:good,w_1440/v1527682422/tobiaswust.de/IMG_1080.jpg"); */
  background-repeat: no-repeat;
  background-position: 60% 0;
  background-attachment: fixed;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  background-size: cover;
}
</style>
