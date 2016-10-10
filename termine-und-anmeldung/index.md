---
layout: page
title: Termine und Anmeldung
scssfile: termine.scss
---
Du hast Dich entschieden den Weg zum Direktzugang mit uns zu gehen?!  
Gute Entscheidung! Versprochen ;-)  
Müssen wir nur noch einen geeigneten Termin für Deine Fortbildung zum sektoralen Heilpraktiker für Physiotherapie finden.  
Unsere aktuellen Termine sind:
{% for kurs in site.data.kurstermine %}
<script type="application/ld+json">
  {% include eventmetadata.json event=kurs %}
  </script>
<div markdown="0" class="kurstermincontainer">
   <div class="kursbackground  {{kurs.color}}"></div>
   <div class="kurstermincontent">
    <span>Kursort: {{kurs.ort}} in {{kurs.land}}</span> <br/>
    <span>Kurstage: {{kurs.datum}}</span> <br/>
    <span>Preis: {{kurs.preis}}</span> <br/>
    <a target="_blank" href="{{kurs.link}}">Hier klicken zur Anmeldung</a>
    </div>
</div>
{% endfor %}
<div class="clearfix"></div>
Hast Du noch keinen passenden Termin gefunden? Keine Sorge, es kommen bald neue.
Bitte schreib uns ruhig direkt [eine Nachricht über unser Kontaktformular]({{site.baeurl}}/kontakt/) und wir informieren Dich sobald neue Termine feststehen.

Die Termine werden üblicherweise zwischen 4 und 8 Monaten im Voraus bekannt gegeben.
Wir sind dabei nicht an einen festen Ort gebunden, sondern in vielen Orten Deutschlands wechselnd unterwegs. So sollte auch für Dich in absehbarer Zeit ein Kurs erreichbar sein. 
Wer es eilig hat, muss vielleicht etwas weiter fahren. Die Reise lohnt sich für Dich.

Zur Zeit sind wir vor allem in Niedersachsen, Nordrhein-Westfalen, Hessen, Rheinland-Pfalz und Bayern unterwegs, um Physiotherapeuten auf dem Weg zum <em>Heilpraktiker Physiotherapie</em> zu begleiten.
 
Für die meisten Teilnehmer der Fortbildung ist es bzgl. der Anerkennung egal, wo diese stattfindet. Sie können also z.B. auch aus Bayern am Kurs in NRW teilnehmen. Für die Anerkennung nach Aktenlage spielt das keine Rolle.


Lediglich Teilnehmer/Innen aus Baden-Württemberg sind in dieser Hinsicht etwas eingeschränkt. 
Die Fortbildung muss, nach internen Richtlinien des Sozialministeriums Baden-Württembergs, in Niedersachsen oder NRW durch staatliche Behörden anerkannt sein und muss auch dort stattgefunden haben. 
Es haben auch schon Teilnehmer aus Baden-Württemberg die Anerkennung erhalten, wenn Sie z.B. unseren Kurs in Rheinland-Pfalz absolviert haben. Wer aber sicher gehen will bzgl. der Anerkennung nach Aktenlage, sollte unsere Kurse in NRW oder Niedersachsen vorziehen. 
Weitere Informationen zu den einzelnen Bundesländern findest Du unter [Voraussetzungen]({{site.baseurl}}/voraussetzungen-und-anerkennung/).

Die Anmeldung erfolgt über unser Online-Anmeldeformular. Klicke dafür einfach oben auf dieser Seite auf den grünen Button bei Deinem gewählten Termin.  
Wer eine staatliche Bildungsförderung wie den Bildungsscheck nutzt, gibt einfach im Formular als Gutschein-Code das Wort "Bildungsscheck" ein.

Die Fortbildung findet zur Zeit immer an 2 mal 3 Tagen statt, von Freitag 12 Uhr bis Sonntag 18 Uhr.
Weitere Informationen zu [unserer Fortbildung zum <em>Heilpraktiker Physiotherapie</em>, findest Du unter Fortbildung]({{site.baseurl}}/fortbildung-zum-heilpraktiker-physiotherapie/).

Falls Du oben auf dieser Seite keinen geeigneten Termin findest, trage Dich doch bitte in [unseren Newsletter "Interessiert an weiteren Kursen" ein](https://www.edoobox.com/de/book/D3.D3.QBhUp2ejQFqSCyQLTPX5QEVOll2hHc7Gg70HtcVF2.hKWYB2.d0mSFORpLbuLj4F2.cnlmlWB9E4B2.VMpZGnqDuRIeNXf/?edref=hppt){:target="_blank"}. Dann wirst Du über alle neuen Termine schnellstmöglich informiert.


