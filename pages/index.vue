<template>
<div>
  <div id="eyecatcher">
  <h1>Devtools4WP</h1>
  <span class="undertext">Nutze die Chrome Devtools für Wordpress</span>
  </div>
</div>
</template>

<script>
export default {
  head: {
    title: "Home",
    meta: [
      {
        hid: "description",
        name: "description",
        content:
          "Hi, ich bin Tobias Wust. Ich bin Fullstack Developer und mache Websites und Progressive Webapps mit Vue und Wordpress. Außerdem programmiere ich mit SAP ABAP."
      }
    ]
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
  text-align: center;
}
</style>
