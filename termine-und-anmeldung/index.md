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
Wir bieten viele Kursorte z.B. in Niedersachsen, Nordrhein-Westfalen, Hessen, Rheinland-Pfalz, Bayern, Berlin und Thüringen unterwegs, um Physiotherapeuten auf dem Weg zum <em>Heilpraktiker Physiotherapie</em> zu begleiten. Hinzu kommen unsere beliebten Onlinekurse, die Du ganz entspannt von Deinem Sofa zuhause aus absolvieren kannst.  
Für die meisten Teilnehmer der Fortbildung ist es bzgl. der Anerkennung egal, wo diese stattfindet. Sie können also z.B. auch aus Bayern am Kurs in NRW teilnehmen. Für die Anerkennung nach Aktenlage spielt das keine Rolle.  Die Vorgaben zur Erlaubniserteilung sind jedoch nicht überall gleich. Genau Informationen dazu erhälst Du unter <a href="{{site.baseurl}}/voraussetzungen-und-anerkennung/">Voraussetzungen</a>.


<amp-iframe id="gmaps" src="https://arnold85.github.io/websiteassets/googlemaps/gmaps.html" width="400" height="400" layout="responsive" frameborder="0" sandbox="allow-forms allow-scripts allow-same-origin"><amp-img layout="fill" src="/assets/images/gmapsplaceholder.jpg" placeholder></amp-img></amp-iframe>  

## Unsere aktuellen Termine sind:

<script type="application/ld+json">
    {
      "@context": "http://schema.org",
      "@type": "ItemList",
      "itemListElement": [
        {% for kurs in site.data.kurstermine %}
        {% include eventmetadata.json event=kurs position=forloop.index %}
        {% endfor %}
      ]
    }
</script>
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
    {% if kurs.abgesagt==true %}
      <div class="abgesagt">Kurs wurde abgesagt</div>
    {% else %}
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

Die Fortbildung findet zur Zeit meist an 2 mal 3 Tagen statt, von Freitag 12 oder 13 Uhr bis 20 Uhr und Samstag und Sonntag je von 9 bis 18 Uhr.
Weitere Informationen zu [unserer Fortbildung zum <em>Heilpraktiker Physiotherapie</em>, findest Du unter Fortbildung]({{site.baseurl}}/fortbildung-zum-heilpraktiker-physiotherapie/).
