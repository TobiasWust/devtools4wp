<template>
<div id="wrap">
  <div id="window1">
    <p><strong>Ein Kurs f&uuml;r jeden!</strong></p>
    <p>Lerne auch als Beginner, wie du ganz einfach die Chrome Devtools benutzen kannst, um dein Wordpress Theme nach deinen Vorstellungen zu stylen.</p>
  </div>

  <div class="row">
    <div id="window3">
      <h2>Du brauchst nur</h2>
      <p>Grundkenntnisse in HTML und CSS<br />Erste Erfahrungen mit Wordpress</p>    
    </div>
    
    <div id="window2">
      <h2>Was werde ich lernen?</h2>
      <ul>
      <li>&Uuml;berblick &uuml;ber die Chrome Developer Tools</li>
      <li>Erstelle eine HTML5 Seite und gestalte sie mithilfe der Devtools</li>
      <li>&Uuml;bertrage die gelernten Konzepte auf ein Wordpress Theme</li>
      <li>Devtools Benutzen, um CSS besser zu verstehen</li>
      <li>Verstehe das Boxmodel</li>
      <li>Animationen f&uuml;r eine lebendige moderne Website</li>
      </ul>
    </div>
  </div>
  
  <div class="sticky"><wu_button/></div>

  <div id="window4">
    <h2>Perfekt<br/> für deinen<br/> Start als</h2>
    <ul><li>Virtuelle Assistenz</li>
    <li>Webentwickler</li>
    <li>Blogger</li>
    <li>Affiliate Marketer</li>
    </ul>
  </div>
  <div id="window5">
    <h2>Inhalt:</h2>
    <p>01 - Einleitung<br />02 - Fenster Anordnen<br />03 - Html5 Seite Anlegen<br />04 - Html5 Seite Anlegen 2<br />05 - Erste Schritte In Den Devtools Und Das Boxmodel<br />06 - Mobile View<br />07 - Media Queries &uuml;bersicht<br />08 - Menu Element Style<br />09 - Menu Background In Css Datei<br />10 - Konkurrierende Eigenschaften Im Computed Tab<br />11 - Eigenschaften Suchen Mit Dem Boxmodel<br />12 - Filesystem<br />13 - Cache Leeren Und Neu Laden<br />14 - Mausrad Zum Zahlen &Auml;ndern<br />15 - Text Shadow Helper<br />16 - Box Shadow Helper<br />17 - &Auml;nderungen Mit Der Konsole Finden<br />18 - Changes Tab<br />19 - Link Farbe &Auml;ndern<br />20 - Hover Im Elemtens Tab<br />21 - Filter Im Elements Tab<br />22 - H&auml;kchen Im Elements Tab<br />23 - Unbekannte R&auml;nder Finden Und Entfernen<br />24 - Benutzt Die Boxansicht<br />25 - Javascript In Der Konsole<br />26 - Neue Wordpress Seite Installieren<br />27 - Wordpress Customizer<br />28 - Chrome Gastmodus<br />29 - Cache Leeren Nicht Vergessen<br />30 - Inhaltsbreite Einstellen<br />31 - Farbige K&auml;sten Zum Testen<br />32 - Devtool Zu Stylesheet<br />33 - Home Seite Anpassen<br />34 - Andere Seiten Anpassen<br />35 - Schriftart &Auml;ndern<br />36 - Site Branding Farbe<br />37 - Rahmen Suchen Und Entfernen<br />38 - Men&uuml; Einf&auml;rben<br />39 - Orientierung Im Css<br />40 - Abschluss Elements Tab<br />41 - Transition<br />42 - Transform<br />43 - Animationstab<br />44 - Snippets<br />45 - Networktab<br />46 - Performance Tab<br />47 - Application Tab<br />48 - Cookies<br />49 - Security Tab<br />50 - Audits Tab<br />51 - Slow 3G<br />52 - Andere Tabs<br />53 - Abschluss</p>
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
</script>

<style scoped>
#wrap {
  display: flex;
  flex-direction: column;
  align-items: center;
}

#window1 {
  margin-top: 1em;
  padding: 1em;
  background-color: white;
  width: 60%;
  min-width: 300px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
}
.row {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  flex-wrap: wrap;
}
#window2 {
  transition: all 1s ease;
  transform: perspective(700px) rotateY(-20deg);
  background-color: #ffefad;
  padding: 1em;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  width: 40%;
  min-width: 300px;
  display: flex;
  margin-top: 4em;
}

#window2:hover {
  transform: rotateY(0);
}

#window3 {
  z-index: -1;
  transform: rotateZ(-5deg);
  width: 40%;
  min-width: 300px;
  color: white;
  background-color: #111;
  padding: 1em;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  font-weight: bold;
  margin-top: 4em;
}

#window4 {
  margin-top: 3em;
  display: flex;
  align-items: center;
  padding: 1em;
  background-color: #ffcc00;
  color: #111;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
}
#window4 ul {
  list-style-type: circle;
}

.sticky {
  position: sticky;
  top: 10px;
  margin-top: 3em;
}

#window5 {
  z-index: -1;
  transition: all 1s ease;
  transform: perspective(1000px) rotateY(20deg);
  color: white;
  text-shadow: 1px 1px 2px #111;
  width: 80%;
  min-width: 300px;
  margin-top: 2em;
}
</style>
