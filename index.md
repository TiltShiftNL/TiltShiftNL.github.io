---
layout: default

title: Innovatie die werkt.<br>Good Public Tech
subtitle: Design software voor de mensen op de werkvloer, op straat en aan het bed.

description: Tiltshift is een design en innovatiebedrijf voor good public tech. We gebruiken software design thinking om samen software te maken. We ontwerpen innovatieve publieke digitale diensten, geven inzicht in processen, en maken handige digitale tools voor ambtenaren.
keywords: digitale transformatie, probleemgedreven innovatie, kwartiermaker, human centered design, software design thinking, service design, lean startup, lean ux, agile development, xp, scrum, labs, apps, projecten, advies, consultancy, publieke sector, mens centraal, common ground, open source

image: /assets/img/foto/IMG_1919.jpg
caption: 'Fixxx discovery "Overlast Rembrandtplein", Gemeente&nbsp;Amsterdam'
---
Techniek dient de mens. Maar verouderde software, processen en structuren zitten vaak behoorlijk in de weg. Zo ontstaan veel problemen. Bij burgers en bedrijven maar zeker ook bij uitvoerende organisaties.

Tiltshift vertrekt vanuit deze problemen. We gebruiken software design thinking om samen met de uitvoerenden op een overzichtelijke en snelle manier passende software te maken. Stapje voor stapje vervangen we zo de starre, verouderde systemen door moderne tools voor op de werkvloer, op straat en aan het bed — snelle innovatie die werkt!

<!-- tools voor op straat -->
<!-- tools op maat -->
<!-- software, processen, organisatie -->
<!-- software design thinking -->
<!-- Fixxx -->
<!-- snelle innovatie die werkt -->
<!-- probleemgedreven innovatie -->
<!-- human centered design -->

<style>
    .label {
      display: inline-block;
      background: #f4b4b4;
      padding: 0 4px;
      font-size: 0.7em;
      color: #1C1C1B;
      border-radius: 0.2em;
    }
  </style>

{% assign collection = site.diensten | sort: 'order' %}
{% for item in collection %}
<h1><a href="{{ item.url }}">{{ item.title }}</a></h1>
<p>
  {{ item.description }}<br>
  {% if item.type %}<span class="label">{{ item.type | downcase }}</span>{% endif %}
  {% for label in item.labels %}<span class="label">{{ label }}</span>{% endfor %}
</p>
{% endfor %}