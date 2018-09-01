<template>
  <div>
    <h1>Über Mich</h1>
    <hr>
    <h2>Willkommen auf meiner Seite!</h2>
    <p>Mein Name ist Tobias Wust. Ich bin ein dauerreisender Entwickler.</p>
    <!-- <img style="float: right; margin: 2em;" src="~/assets/img/serioesesfoto.jpg"> -->
    <img style="float: right; margin: 2em;" src="https://res.cloudinary.com/tobiaswust/image/upload/c_scale,e_improve,f_auto,q_auto:good,r_21,w_250/v1527682175/tobiaswust.de/Bewerbungsfoto.jpg">
    
    <h2>Was bedeutet es, ein reisender Entwickler zu sein?</h2>
    <p>Für mich bedeutet es vor allem die Freiheit immer mit meinem Laptop unterwegs zu sein und zu arbeiten wann und wo es mir passt. Ich muss nicht mit Anzug ins Büro und kann sein wer ich gerne bin. Ich begegne dir auf freundschaftliche Art und halte nichts vom "Sie" – dafür bin ich ein Befürworter von langer Zusammenarbeit und bleibe auch gerne mit dir in Kontakt, wenn wir gerade keine gemeinsamen Projekte haben.</p>
    <p>Für dich bedeutet das, dass du in mir einen stets gut gelaunten und motivierten Arbeitspartner findest, der Kunden nicht als Massenware sieht und jedes Problem individuell angeht. Es bedeutet aber auch, dass ich manchmal auf einem Berg ohne Internetverbindung bin.</p>

    <h2>Wer bin ich?</h2>
    <p>Schon seit meinem 11. Lebensjahr war ich irgendwie Informatiker. Am Anfang wollte ich natürlich Spiele entwickeln und habe deshalb meine ersten Schritte mit Textadventures in BASIC gemacht. Darauf folgte Delphi, HTML und vieles mehr.
    Nach der Schule habe ich ein duales Studium in Wirtschaftsinformatik gemacht. In dieser Zeit habe ich dann auch das Reisen für mich entdeckt. Nach dem Studium bin ich deshalb für ein Jahr um die Welt gereist - Alles dazu findest du in meinem <a href="https://wust.me/">privaten Blog</a>.
    Nach dieser Reise habe ich ein paar Jahre als SAP Programmierer im öffentlichen Dienst gearbeitet, bis ich mich irgendwann getraut habe meinen Job und meine Wohnung zu kündigen. Nun bin ich hier.</p>

    <h2>Lebenslauf</h2>
    <h3>Berufserfahrung</h3>
    <ul>
      <li>03/2018 - heute <br><strong>Freelance Developer</strong><br>Websites, Webapps, Games, SAP ABAP</li>
      <li>07/2016 - 06/2018 <br><strong>Remedyne GmbH</strong><br>SAP Anwendungsentwicklung, SAP Anwendungsübersetzung</li>
      <li>09/2013 - 07/2017 <br><strong>Landeshauptstadt Hannover</strong><br>SAP Administration, Anwendungsentwicklung und Modulbetreuung: Berechtigungen, CML, Geschäftspartner</li>
      <li>06/2012 - 09/2012 <br><strong>Landeshauptstadt Hannover</strong><br>Datenbankadministration MySQL, MSSQL</li>
    </ul>

    <h3>Akademische Ausbildung</h3>
    <ul>
      <li>11/2015 - 02/2017 <br><strong>Online-Schule für Gestaltung</strong><br>Fernstudium Grafikdesign</li>    
      <li>08/2009 - 08/2012 <br><strong>Leibniz Fachhochschule</strong><br>B.Sc. Wirtschaftsinformatik 2,3</li>
      <li>bis 07/2009 <br><strong>Gymnasium Langenhagen</strong><br>Abitur 2,8</li>
    </ul>

    <a href="/Tobias_Wust_Lebenslauf_2018_06.pdf">Mein ganzer Lebenslauf als PDF</a>

    <h3>Finde mich</h3>
    <ul>
      <li>Privater Blog: <a href="https://wust.me">wust.me</a></li>
      <li>Xing: <a href="https://www.xing.com/profile/Tobias_Wust">xing.com/profile/Tobias_Wust</a></li>
      <li>Github: <a href="https://github.com/TobiasWust">github.com/TobiasWust</a></li>
      <li>Codepen: <a href="https://codepen.io/tobiaswust/">codepen.io/tobiaswust</a></li>
      <li>LinkedIn: <a href="https://www.linkedin.com/in/tobias-wust">linkedin.com/in/tobias-wust</a></li>      
    </ul>

  </div>
</template>

<script>
export default {
  head: {
    title: "Über Mich",
    meta: [
      {
        hid: "description",
        name: "description",
        content:
          "Hi, ich bin Tobias Wust - ein reisender Entwickler. Das bedeutet, dass ich in meinem Auto lebe und unterwegs als Fullstack Developer arbeite. Hier findest du meinen Lebenslauf."
      }
    ]
  }
};
</script>

<style scoped>
strong {
  color: #f68714;
}

li {
  list-style: circle;
  margin-bottom: 0.5em;
}
</style>