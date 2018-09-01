<template>
<div>
  <h1>Hi, ich bin<br>TOBIAS WUST</h1>
  <p>Ich mache
    <nuxt-link to="/offer/">
    <span class="slider">
      <span class="slide">Websites</span>
      <span class="slide">Progressive Webapps</span>
      <span class="slide">SAP ABAP</span>
    </span></nuxt-link></p>
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
.slider {
  width: 200px;
  display: flex;
  overflow-x: hidden;
  background-color: #f68714;
  align-items: center;
  transition: all 1s;
}

.slider:hover {
  background-color: #3dba6a;
}

@keyframes slide {
  0%,
  20% {
    transform: translateX(0px);
  }
  40%,
  60% {
    transform: translateX(-200px);
  }
  80%,
  100% {
    transform: translateX(-400px);
  }
}

.slide {
  animation: slide 8s ease-in-out 2s infinite alternate;
  width: 200px;
  flex-shrink: 0;
  text-align: center;
}
a {
  color: white;
  text-decoration: none;
}
div {
  color: white;
  font-size: 150%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 70vh;
}

h1 {
  color: white;
  text-align: left;
  font-size: 8vw;
}

h1 {
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
}
</style>
