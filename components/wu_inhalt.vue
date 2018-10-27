<template>
    <ol class="counter">
      <li>Einleitung</li>
      <li>Fenster Anordnen	</li>
      <li>Html5 Seite Anlegen	</li>
      <li>Html5 Seite Anlegen 2	</li>
      <li>Erste Schritte In Den Devtools Und Das Boxmodel	</li>
      <li>Mobile View	</li>
      <li>Media Queries übersicht	</li>
      <li>Menu Element Style	</li>
      <li>Menu Background In Css Datei	</li>
      <li>Konkurrierende Eigenschaften Im Computed Tab	</li>
      <li>Eigenschaften Suchen Mit Dem Boxmodel	</li>
      <li>Filesystem	</li>
      <li>Cache Leeren Und Neu Laden	</li>
      <li>Mausrad Zum Zahlen Ändern	</li>
      <li>Text Shadow Helper	</li>
      <li>Box Shadow Helper	</li>
      <li>Änderungen Mit Der Konsole Finden	</li>
      <li>Changes Tab	</li>
      <li>Link Farbe Ändern	</li>
      <li>Hover Im Elemtens Tab	</li>
      <li>Filter Im Elements Tab	</li>
      <li>Häkchen Im Elements Tab	</li>
      <li>Unbekannte Ränder Finden Und Entfernen	</li>
      <li>Benutzt Die Boxansicht	</li>
      <li>Javascript In Der Konsole	</li>
      <li>Neue Wordpress Seite Installieren	</li>
      <li>Wordpress Customizer	</li>
      <li>Chrome Gastmodus	</li>
      <li>Cache Leeren Nicht Vergessen	</li>
      <li>Inhaltsbreite Einstellen	</li>
      <li>Farbige Kästen Zum Testen	</li>
      <li>Devtool Zu Stylesheet	</li>
      <li>Home Seite Anpassen	</li>
      <li>Andere Seiten Anpassen	</li>
      <li>Schriftart Ändern	</li>
      <li>Site Branding Farbe	</li>
      <li>Rahmen Suchen Und Entfernen	</li>
      <li>Menü Einfärben	</li>
      <li>Orientierung Im Css	</li>
      <li>Abschluss Elements Tab	</li>
      <li>Transition	</li>
      <li>Transform	</li>
      <li>Animationstab	</li>
      <li>Snippets	</li>
      <li>Networktab	</li>
      <li>Performance Tab	</li>
      <li>Application Tab	</li>
      <li>Cookies	</li>
      <li>Security Tab	</li>
      <li>Audits Tab	</li>
      <li>Slow 3G	</li>
      <li>Andere Tabs	</li>
      <li>Abschluss	</li>
    </ol>
</template>

<script>
export default {
  name: "wu_inhalt"
};
</script>

<style scoped>
.counter {
  list-style: none;
  display: grid;
  grid-row-gap: 1em;
  grid-template-columns: repeat(2, 1fr);
}
.counter li {
  padding-top: 0.5em;
  padding-left: 2em;
  margin-right: 3em;
  position: relative;
  counter-increment: count;
  z-index: 90;
  border-top: 2px solid #fc0;
}
.counter li::before {
  content: counter(count);

  background: #ffcc00;
  color: #111;

  font-size: 1.5em;
  font-weight: 700;
  font-style: italic;
  border-radius: 50%;
  text-align: center;
  padding-left: 2.25%;
  left: -1em;
  top: -0.1em;
  height: 1.35em;
  width: 1.35em;
  position: absolute;
  z-index: -1;
}
</style>