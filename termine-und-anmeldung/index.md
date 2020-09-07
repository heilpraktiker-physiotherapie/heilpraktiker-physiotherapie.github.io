---
layout: page
title: Termine und Anmeldung zur Fortbildung sektoraler Heilpraktiker Physiotherapie
metatitle: Termine zur Fortbildung sektoraler Heilpraktiker Physiotherapie
description: Termine und Anmeldeformular zur Fortbildung Heilpraktiker für Physiotherapie
scssfile: termine.scss
customamp:
    - amp-iframe
---
Du hast Dich entschieden den Weg zum Direktzugang mit uns zu gehen?!  
Gute Entscheidung! Versprochen ;-)  
Müssen wir nur noch einen geeigneten Termin für Deine Fortbildung zum sektoralen Heilpraktiker für Physiotherapie finden.  
Zur Zeit sind wir vor in Niedersachsen, Nordrhein-Westfalen, Hessen, Rheinland-Pfalz, Bayern, Berlin und Thüringen unterwegs, um Physiotherapeuten auf dem Weg zum <em>Heilpraktiker Physiotherapie</em> zu begleiten.  
<amp-iframe id="gmaps" src="https://arnold85.github.io/websiteassets/googlemaps/gmaps.html" width="400" height="400" layout="responsive" frameborder="0" sandbox="allow-forms allow-scripts allow-same-origin"><amp-img layout="fill" src="/assets/images/gmapsplaceholder.jpg" placeholder></amp-img></amp-iframe>  

Für die meisten Teilnehmer der Fortbildung ist es bzgl. der Anerkennung egal, wo diese stattfindet. Sie können also z.B. auch aus Bayern am Kurs in NRW teilnehmen. Für die Anerkennung nach Aktenlage spielt das keine Rolle.  
<div class="achtungbox fullwidthtextbar">
  <strong>Mit uns sicher planen und die individuell optimale Schulungsform auswählen:</strong>  
  Da wir alle nicht in die Zukunft sehen können und unklar bleibt, wie sich die Einschränkungen wegen Covid-19 entwickeln, können die Kurse evtl. nicht als Präsenzveranstaltung stattfinden. Mit uns kannst Du aber sicher planen.  
  Wir haben hervorragende Erfahrung mit der Durchführung des Kurses als Onlineseminar gemacht. Wenn die Präsenzkurse also nicht wie geplant möglich sein sollte, wechseln wir in die digitale Welt und liefern Dir dort die beste Fortbildung zum Heilpraktiker für Physiotherapie. Diese wird genauso von den Gesundheitsämtern anerkannt, wie die Präsenzveranstaltung.  
  Langfristig sollen unsere Teilnehmer*innen das beste aus beiden Welten mitnehmen können. Es wird Kurse geben,  
  <ul>
    <li>in denen der gesamte vorgeschriebene Unterricht ganz traditionell in Präsenz stattfindet</li> 
    <li>andere kombinierte Kurse, welche einen großen Teil der Theorie als Webinar vermitteln und ein Wochenende eher praktische Inhalte in Präsenz üben lassen</li> 
    <li>und weitere Kurse, die vollständig, bis auf die schriftliche Abschlussprüfung, bequem von zuhause aus durchgeführt werden können.</li>
  </ul>  
  So sollte für jeden Lerntyp und jede Lebenssituation das perfekte Format dabei sein.
</div>
Unsere aktuellen Termine sind:
{% for kurs in site.data.kurstermine %}
<script type="application/ld+json">
      {% include eventmetadata.json event=kurs %}
</script>
{% endfor %}
{% assign var bgcolor = 'green' %}
{% for kurs in site.data.kurstermine %}
{% if kurs.show == true %}
<div markdown="0" class="kurstermincontainer">
   {% if forloop.first == true %}
        {% assign bgcolor = 'green' %}
    {% elsif bgcolor == 'green' %}
        {% assign bgcolor = 'blue' %}
    {% elsif bgcolor == 'blue' %}
        {% assign bgcolor = 'red' %}
    {% elsif bgcolor == 'red' %}
        {% assign bgcolor = 'green' %}
  {% endif %}
   <div class="kursbackground  {{bgcolor}}"></div>
   <div class="kurstermincontent">
   {% if kurs.elearning==true and kurs.ort  %}
   <span>Prüfungsort(e): {{kurs.ort}}</span> <br/>
   {% elsif  kurs.elearning==true%}
  <span>Kursort: <b>E-learning von beliebigem Ort</b> </span> <br/>
   {% elsif  kurs.ort%}
  <span>Kursort: <b>{{kurs.ort}}</b> in {{kurs.land}}</span> <br/>
   {% endif %}
    <span>Kurstage: {{kurs.datum}}</span> <br/>
    {% if kurs.ablauf %}
    <span><small>Ablauf: {{kurs.ablauf}}</small></span> <br/>
    {% endif %}
    <span>Veranstalter: {{kurs.veranstalter}}</span> <br/>
    {% if kurs.fruehbucher %}
      <span>Frühbucherpreis: {{kurs.fruehbucher}}€ bis {{kurs.fruehbucherdatum}} (begrenzte Plätze)</span> <br/>
    {% endif %}
    {% if kurs.preislink %}
      <span>Preis: Infos auf <a target="_blank" href="{{kurs.preislink}}">Seite des Veranstalters</a></span> <br/>
        {% elsif kurs.preis %}
            <span>Preis: {{kurs.preis}}€</span> <br/>
    {% endif %}
    <a target="_blank" href="{{kurs.link}}" class="anmelde_link">Hier klicken zur Anmeldung</a>
    {% if kurs.elearning==true %}
      <div class="iselearning">E-Learning</div>
    {% elsif kurs.elearning==false %}
      <div class="ispresence">Präsenzkurs</div>
    {% elsif kurs.elearning=='hybrid' %}
      <div class="ishybrid">Hybrid: E-Learning und Präsenzkurs</div>
    {% endif %}
    {% if kurs.warteliste==true %}
      <div class="warteliste">Warteliste</div>
    {% endif %}
    </div>
</div>
{% endif %}
{% endfor %}
<div class="clearfix"></div>
Hast Du noch keinen passenden Termin gefunden? Keine Sorge, es kommen bald neue.
Bitte schreib uns ruhig direkt [eine Nachricht]({{site.baseurl}}/kontakt/) und wir informieren Dich sobald neue Termine feststehen.

Die Termine werden üblicherweise zwischen 4 und 8 Monaten im Voraus bekannt gegeben.
Wir sind dabei nicht an einen festen Ort gebunden, sondern in vielen Orten Deutschlands wechselnd unterwegs. So sollte auch für Dich in absehbarer Zeit ein Kurs erreichbar sein.  
Wer es eilig hat, muss vielleicht etwas weiter fahren. Die Reise lohnt sich für Dich.

Weitere Informationen zu den zu den Anforderungen für den Heilpraktiker Physiotherapie in einzelnen Bundesländern, findest Du unter [Voraussetzungen]({{site.baseurl}}/voraussetzungen-und-anerkennung/).

Bei einigen Kursen arbeiten wir mit externen Fortbildungsanbietern zusammen. Bei diesen Kursen findet die Anmeldung über deren jeweilige Systeme statt.  
Andere Kurse werden von uns selbst organisiert. Die Anmeldung erfolgt dann über unser Online-Anmeldeformular. Klicke dafür einfach oben auf dieser Seite auf den grünen Button bei Deinem gewählten Termin.  
Wer eine staatliche Bildungsförderung wie den Bildungsscheck nutzt, gibt einfach im Formular als Gutschein-Code das Wort "Bildungsscheck" ein.

Die Fortbildung findet zur Zeit meist an 2 mal 3 Tagen statt, von Freitag 12 oder 13 Uhr bis 20 Uhr und Samstag und Sonntag je von 9 bis 18 Uhr.
Weitere Informationen zu [unserer Fortbildung zum <em>Heilpraktiker Physiotherapie</em>, findest Du unter Fortbildung]({{site.baseurl}}/fortbildung-zum-heilpraktiker-physiotherapie/).
