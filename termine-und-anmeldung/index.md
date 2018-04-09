---
layout: page
title: Termine und Anmeldung
description: Termine und Anmeldeformular zur Fortbildung Heilpraktiker für Physiotherapie
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
{% endfor %}
{% for kurs in site.data.kurstermine %}
<div markdown="0" class="kurstermincontainer">
   <div class="kursbackground  {{kurs.color}}"></div>
   <div class="kurstermincontent">
    <span>Kursort: {{kurs.ort}} in {{kurs.land}}</span> <br/>
    <span>Kurstage: {{kurs.datum}}</span> <br/>
    <span>Veranstalter: {{kurs.veranstalter}}</span> <br/>
    {% if kurs.fruehbucher %}
      <span>Frühbucherpreis: {{kurs.fruehbucher}} bis {{kurs.fruehbucherdatum}} (begrenzte Plätze)</span> <br/>
    {% endif %}
    {% if kurs.preis %}
      <span>Preis: {{kurs.preis}}</span> <br/>
    {% endif %}
    {% if kurs.preislink %}
      <span>Preis: Infos auf <a target="_blank" href="{{kurs.preislink}}">Seite des Veranstalters</a></span> <br/>
    {% endif %}
    <a target="_blank" href="{{kurs.link}}" class="anmelde_link">Hier klicken zur Anmeldung</a>
    {% if kurs.warteliste==true %}
      <div class="warteliste">Warteliste</div>
    {% endif %} 
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

Bei einigen Kursen arbeiten wir mit externen Fortbildungsanbietern zusammen. Bei diesen Kursen findet die Anmeldung über deren jeweilige Systeme statt.  
Andere Kurse werden von uns selbst organisiert. Die Anmeldung erfolgt dann über unser Online-Anmeldeformular. Klicke dafür einfach oben auf dieser Seite auf den grünen Button bei Deinem gewählten Termin.  
Wer eine staatliche Bildungsförderung wie den Bildungsscheck nutzt, gibt einfach im Formular als Gutschein-Code das Wort "Bildungsscheck" ein.

Die Fortbildung findet zur Zeit immer an 2 mal 3 Tagen statt, von Freitag 12 Uhr bis Sonntag 18 Uhr.
Weitere Informationen zu [unserer Fortbildung zum <em>Heilpraktiker Physiotherapie</em>, findest Du unter Fortbildung]({{site.baseurl}}/fortbildung-zum-heilpraktiker-physiotherapie/).



