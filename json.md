---
layout: page
title: Implementacion de Json
description: Json con jugadores y raperos
featured_image: json.jpg
---

{% for jugador in site.data.jugadores.players %} 
    {% if jugador.age < 30 %}
        <p>{{ jugador.name | upcase }} {{ jugador.song }}</p>
    {% endif %}
{% endfor %}

{% for rapero in site.data.raperos.rappers %} 
    {% if rapero.age > 30 %}
        <p>{{ rapero.real_name }} {{ rapero.nba_song }} {{ rapero.artist_name }}</p>
    {% endif %}
{% endfor %}
