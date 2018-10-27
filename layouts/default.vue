<template>
  <div class="wrapper">
      <header><eyecatcher/></header>
      <article class="content">      
          <nuxt/>
      </article>
    <footer class="footer"><wu_footer/></footer>
    <cookienotice />
  </div>
</template>

<script>
import cookienotice from "~/components/cookienotice.vue";
import eyecatcher from "~/components/eyecatcher.vue";
import wu_footer from "~/components/wu_footer.vue";
import { mapState } from "vuex";

export default {
  data() {
    return {};
  },
  components: {
    cookienotice,
    eyecatcher,
    wu_footer
  },
  computed: mapState(["page"])
};
</script>

<style>
body {
  overflow: scroll;
  margin: 0;
  font-family: "Roboto", "sans-serif";
  background-color: #fff;
  color: #111;
  /* font-size: 130%; */
  min-height: 100vh;
}

body:before {
  content: "";
  display: block;
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  height: 100vh;
  z-index: -20;
  background-image: url("~/assets/img/background_sw.png");
  /* background-image: url("https://res.cloudinary.com/tobiaswust/image/upload/c_scale,f_auto,q_auto:good,w_1440/v1527682422/tobiaswust.de/IMG_1080.jpg"); */
  background-repeat: no-repeat;
  background-position: 60% 0;
  background-attachment: fixed;
  background-size: cover;
}

/* @media (max-width: 1024px) {
  #body:before {
    background-image: url("~/assets/img/background.png");
  }
} */

h1 {
  color: #111;
  text-align: center;
  margin: 0 0 0 0;
}
h2 {
  color: #888;
}
h1,
h2 {
  font-family: "Neuton", "serif";
}

hr {
  border: 0;
  height: 2px;
  background-image: linear-gradient(
    to right,
    rgba(0, 0, 0, 0),
    #ffcc00,
    rgba(0, 0, 0, 0)
  );
  width: 30%;
}

.content {
  flex: 1;
}

footer {
  width: 100%;
  bottom: 0px;
}

a {
  color: #111;
  text-decoration-color: #ffcc00;
}

a:hover {
  color: #ffcc00;
}

.material {
  box-shadow: 0 3px 3px 0 rgba(0, 0, 0, 0.14), 0 2px 7px 0 rgba(0, 0, 0, 0.12),
    0 5px 3px -5px rgba(0, 0, 0, 0.2);
}
</style>


