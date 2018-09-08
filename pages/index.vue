<template>
<div id="wrap">
  <section id="shortsummary">
    <h2>Ein Kurs f&uuml;r jeden!</h2>
    <p>Lerne in diesem <strong>zweistündigen Videokurs</strong> auch als Beginner, wie du ganz <strong>einfach</strong> die Chrome Devtools benutzen kannst, um dein <strong>Wordpress Theme nach deinen Vorstellungen zu stylen</strong>.</p>
  </section>

    <wu_button/>

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
      <div><img src="~/assets/img/screenshot.jpg"></div>
    </section>

  <section id="inhalt">
    <h2>Inhalt:</h2>
    <p>01 - Einleitung<br />02 - Fenster Anordnen<br />03 - Html5 Seite Anlegen<br />04 - Html5 Seite Anlegen 2<br />05 - Erste Schritte In Den Devtools Und Das Boxmodel<br />06 - Mobile View<br />07 - Media Queries &uuml;bersicht<br />08 - Menu Element Style<br />09 - Menu Background In Css Datei<br />10 - Konkurrierende Eigenschaften Im Computed Tab<br />11 - Eigenschaften Suchen Mit Dem Boxmodel<br />12 - Filesystem<br />13 - Cache Leeren Und Neu Laden<br />14 - Mausrad Zum Zahlen &Auml;ndern<br />15 - Text Shadow Helper<br />16 - Box Shadow Helper<br />17 - &Auml;nderungen Mit Der Konsole Finden<br />18 - Changes Tab<br />19 - Link Farbe &Auml;ndern<br />20 - Hover Im Elemtens Tab<br />21 - Filter Im Elements Tab<br />22 - H&auml;kchen Im Elements Tab<br />23 - Unbekannte R&auml;nder Finden Und Entfernen<br />24 - Benutzt Die Boxansicht<br />25 - Javascript In Der Konsole<br />26 - Neue Wordpress Seite Installieren<br />27 - Wordpress Customizer<br />28 - Chrome Gastmodus<br />29 - Cache Leeren Nicht Vergessen<br />30 - Inhaltsbreite Einstellen<br />31 - Farbige K&auml;sten Zum Testen<br />32 - Devtool Zu Stylesheet<br />33 - Home Seite Anpassen<br />34 - Andere Seiten Anpassen<br />35 - Schriftart &Auml;ndern<br />36 - Site Branding Farbe<br />37 - Rahmen Suchen Und Entfernen<br />38 - Men&uuml; Einf&auml;rben<br />39 - Orientierung Im Css<br />40 - Abschluss Elements Tab<br />41 - Transition<br />42 - Transform<br />43 - Animationstab<br />44 - Snippets<br />45 - Networktab<br />46 - Performance Tab<br />47 - Application Tab<br />48 - Cookies<br />49 - Security Tab<br />50 - Audits Tab<br />51 - Slow 3G<br />52 - Andere Tabs<br />53 - Abschluss</p>
  </section>
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
  },
  head: {
    title: "Home",
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
  background-color: white;
  width: 80%;
  min-width: 300px;
}

#shortsummary {
  text-align: justify;
  margin-top: 1em;
  padding: 1em;
  background-color: white;
  min-width: 300px;
}
.row {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  flex-wrap: wrap;
  width: 100%;
  background-color: #eee;
  padding: 2em 0;
}
#question {
  text-align: justify;
  margin-top: 1em;
  padding: 1em;
  background-color: white;
  min-width: 300px;
  display: flex;
  justify-content: space-around;
}
#question div {
  transform: rotateZ(20deg);
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
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

.sticky {
  position: sticky;
  top: 1em;
  margin-top: 3em;
}

#inhalt {
  width: 100%;
  display: flex;
  color: white;
  text-shadow: 1px 1px 2px #111;
  min-width: 300px;
  margin-top: 2em;
  background-color: #111;
  flex-direction: column;
  align-items: center;
}
</style>
