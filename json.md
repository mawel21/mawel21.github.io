---
layout: page
title: Implementacion de Json
description: Json con jugadores y raperos
featured_image: json.jpg
---

<h3>Jugadores menores de 30 años</h3>
<ul>
{% for jugador in site.data.jugadores.players %}
    {% if jugador.age < 30 %}
        <li><b>{{ jugador.name | upcase }}</b> - {{ jugador.song }}</li>
    {% endif %}
{% endfor %}
</ul>

<h3>Raperos mayores de 30 años</h3>
<ul>
{% for rapero in site.data.raperos.rappers %}
    {% if rapero.age > 30 %}
        <li><b>{{ rapero.real_name }}</b> ({{ rapero.artist_name }}) - {{ rapero.nba_song }}</li>
    {% endif %}
{% endfor %}
</ul>

<h3>Raperos y sus referencias a la NBA</h3>
<ul>
{% for rapero in site.data.raperos.rappers %}
    <li>
        <b>{{ rapero.artist_name }}</b> - "{{ rapero.nba_song }}"  
        <br>Información: {{ rapero.information }}
    </li>
{% endfor %}
</ul>

