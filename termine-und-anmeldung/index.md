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
Wir bieten viele Kursorte z.B. in Niedersachsen, Nordrhein-Westfalen, Hessen, Rheinland-Pfalz, Bayern und Thüringen, um Physiotherapeuten auf dem Weg zum <em>Heilpraktiker Physiotherapie</em> zu begleiten. Hinzu kommen unsere beliebten Onlinekurse, die Du ganz entspannt von Deinem Sofa zuhause aus absolvieren kannst.  
Für die meisten Teilnehmer der Fortbildung ist es bzgl. der Anerkennung egal, wo diese stattfindet. Sie können also z.B. auch aus Bayern am Kurs in NRW teilnehmen. Für die Anerkennung nach Aktenlage spielt das keine Rolle.  Die Vorgaben zur Erlaubniserteilung sind jedoch nicht überall gleich. Genau Informationen dazu erhälst Du unter <a href="{{site.baseurl}}/voraussetzungen-und-anerkennung/">Voraussetzungen</a>.


<amp-iframe id="gmaps" src="https://arnold85.github.io/websiteassets/googlemaps/gmaps.html" width="400" height="400" layout="responsive" frameborder="0" sandbox="allow-forms allow-scripts allow-same-origin"><amp-img layout="fill" src="{{site.baseurl}}/assets/images/webP/gmapsplaceholder.webp" placeholder></amp-img></amp-iframe>  

## Unsere aktuellen Termine sind:

<script type="application/ld+json">
    {
      "@context": "http://schema.org",
      "@type": "ItemList",
      "itemListElement": [
      {% assign firstEntry = true -%}
        {% for kurs in site.data.kurstermine -%}
          {% if kurs.show == true -%}
            {% if forloop.first == false and firstEntry == false -%}
              {{","}}
            {% endif -%}
            {% assign firstEntry = false -%}
            {% include eventmetadata.json event=kurs position=forloop.index %}
          {% endif -%}
        {% endfor -%}
      ]
    }
</script>
{% assign var bgcolor = 'midgray' %}
{% for kurs in site.data.kurstermine %}
{% if kurs.show == true %}
<div id="{{ kurs.kursnummer }}" markdown="0" class="kurstermincontainer">
   {% if forloop.first == true %}
        {% assign bgcolor = 'midgray' %}
    {% elsif bgcolor == 'midgray' %}
        {% assign bgcolor = 'lightgray' %}
    {% elsif bgcolor == 'lightgray' %}
        {% assign bgcolor = 'midgray' %}
  {% endif %}
   <div class="kursbackground {{ bgcolor }}"></div>
  <div class="kurstermincontent">
  <details>
    <summary>
   {% if kurs.courseMode == 'Online' %}
   <span>Kursort: <b>E-learning von beliebigem Ort</b></span> <br/>
   {% elsif kurs.ort %}
   <span>Kursort: <b>{{ kurs.ort }}</b> in {{ kurs.land }}</span> <br/>
   {% endif %}
    <span>Kurstage: {{ kurs.datum }}</span> <br/>
    {% if kurs.courseMode == 'Online' %}
          <div class="iselearning">Webinar</div>
        {% elsif kurs.courseMode == 'Onsite' %}
          <div class="ispresence">Präsenzkurs</div>
        {% elsif kurs.courseMode == 'Blended' %}
          <div class="ishybrid">Blended: Webinar und Präsenzkurs</div>
        {% endif %}
        </summary>
            {% if kurs.ablauf %}
    <span><small>Ablauf: {{ kurs.ablauf }}</small></span> <br/>
    {% endif %} 
    <span>Veranstalter: {{ kurs.veranstalter }}</span> <br/>
    {% if kurs.abgesagt == true %}
      <div class="abgesagt">Kurs wurde abgesagt</div>
    {% else %}
        {% if kurs.fruehbucher  and kurs.fruehbucher != empty%}
          <span>Frühbucherpreis: {{ kurs.fruehbucher }}€ bis {{ kurs.fruehbucherdatum }} (begrenzte Plätze)</span> <br/>
        {% endif %}
        {% if kurs.preislink  and kurs.preislink != empty%}
          <span>Preis: Infos auf <a target="_blank" href="{{ kurs.preislink }}" class="box-link">Seite des Veranstalters</a></span> <br/>
        {% elsif kurs.preis %}
          <span>Preis: {{ kurs.preis }}€</span> <br/>
        {% endif %}
        <a target="_blank" href="{{ kurs.enrollmentLink }}" class="anmelde_link  box-link">Hier klicken zur Anmeldung</a>
       
        {% if kurs.warteliste == true %}
          <div class="warteliste">Warteliste</div>
        {% endif %}
    {% endif %}
   </details>
   
    
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
