<template>
<div id="wrap">
  <section id="shortsummary">
    <h2>Ein Kurs f&uuml;r jeden!</h2>
    <p>Lerne in diesem <strong>zweistündigen Videokurs</strong> auch als Beginner, wie du ganz <strong>einfach</strong> die Chrome Devtools benutzen kannst, um dein <strong>Wordpress Theme nach deinen Vorstellungen zu stylen</strong>.</p>
  </section>

    <div class="button"><wu_button/></div>

  <div class="row">
    <section id="requirements">
      <h2>Du brauchst nur</h2>
      <p>Grundkenntnisse in HTML und CSS<br />Erste Erfahrungen mit Wordpress</p>    
    </section>  
      <section id="window4">
    <h2>Perfekt<br/> für deinen<br/> Start als</h2>
    <ul><li>Virtuelle Assistenz</li>
    <li>Webentwickler</li>
    <li>Blogger</li>
    <li>Affiliate Marketer</li>
    </ul>
  </section>
  </div>
  
    <section id="question">
      <h2>Was werde ich lernen?</h2>
      <ul>
        <li>&Uuml;berblick &uuml;ber die Chrome Developer Tools</li>
        <li>Erstelle eine HTML5 Seite und gestalte sie mit Hilfe der Devtools</li>
        <li>&Uuml;bertrage die gelernten Konzepte auf ein Wordpress Theme</li>
        <li>Devtools benutzen, um CSS besser zu verstehen</li>
        <li>Verstehe das Boxmodel</li>
        <li>Animationen f&uuml;r eine lebendige moderne Website</li>
      </ul>
    </section>

    <section id="youtube">
      <h2>Kostenlose Vorschau</h2>
      <p>Ich habe für dich die <strong><a href="https://youtu.be/pZ1RaFIdeSY" target="_blank">ersten 5 Videos auf Youtube</a></strong> gestellt. Guck sie dir doch mal an und entscheide dann!</p>
      <a href="https://youtu.be/pZ1RaFIdeSY" target="_blank">
        <img alt="Youtube Vorschau" src="https://res.cloudinary.com/tobiaswust/image/upload/f_auto,q_auto/v1540666605/devtools4wp/devtools4wp_youtube.png" />
      </a>
      <p><small>Wenn du auf das Bild klickst öffnest du Youtube in einem neuen Fenster</small></p>
    </section>
  
  <div class="button"><wu_button/></div>
  
  <section id="inhalt">
    <h2>Inhalt:</h2>
    <wu_inhalt/>
    
  </section>
  <div class="button"><wu_button/></div>
</div>
</template>

<script>
import wu_button from "~/components/wu_button.vue";
import wu_inhalt from "~/components/wu_inhalt.vue";

export default {
  data() {
    return {};
  },
  components: {
    wu_button,
    wu_inhalt
  },
  head: {
    //title: "Home",
    titleTemplate: "Devtools4WP - Nutze die Chome Devtools für Wordpress",
    meta: [
      {
        hid: "description",
        name: "description",
        content:
          "Lerne auch als Beginner, wie du ganz einfach die Chrome Devtools benutzen kannst, um dein Wordpress Theme nach deinen Vorstellungen zu stylen."
      }
    ]
  }
};
</script>

<style scoped>
#wrap {
  margin: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  /* background-color: rgba(250, 250, 250, 0.5); */
  min-width: 300px;
  width: 80%;
}

#shortsummary {
  margin-top: 2em;
  width: 100%;
  padding: 1em;
  box-sizing: border-box;
  background-color: white;
  min-width: 300px;
}
#shortsummary h2,
#shortsummary p {
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}

@media (max-width: 1024px) {
  #wrap {
    width: 100%;
  }
  #shortsummary h2,
  #shortsummary p {
  width: 100%;
  }
}

.row {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  flex-wrap: wrap;
  width: 100%;
  background-color: #eee;
}
#question {
  text-align: justify;
  margin-top: 1em;
  padding: 1em;
  background-color: white;
  min-width: 300px;
  display: flex;
  justify-content: space-around;
  transform: rotateZ(-5deg);
}

#requirements {
  margin: 0.5em 0;
  /* transform: rotateY(0deg); */
  color: rgba(255, 255, 255);
  background-color: #111;
  padding: 1em;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  align-self: stretch;
  min-width: 300px;
}

#window4 {
  margin: 0.5em 0;
  font-weight: bold;
  display: flex;
  align-items: center;
  padding: 1em;
  background-color: #ffcc00;
  color: #111;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  min-width: 300px;
}
#window4 ul {
  list-style-type: circle;
}

.button {
  /* position: sticky;
  top: 0; */
  margin-top: 3em;
  margin-bottom: 3em;
}

#inhalt {
  width: 100%;
  display: flex;
  color: white;
  text-shadow: 1px 1px 2px #111;
  min-width: 300px;
  background-color: #111;
  flex-direction: column;
  align-items: center;
  padding-top: 1em;
}

#youtube {
  margin-top: 2em;
  width: 100%;
  padding: 1em;
  box-sizing: border-box;
  background-color: #eee;
  text-align: center;
}
#youtube img {
  transform: scale(0.95);
  max-width: 80vw;
  transition: all 0.3s ease;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
}
#youtube img:hover {
  transform: scale(1);
  transform: rotateZ(1deg);
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.8);
}

h2 {
  margin-top: 0;
}

section,
.row {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
}
</style>
