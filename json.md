---
layout: page
title: Implementacion de Json
description: Json con jugadores y raperos
featured_image: json.jpg
---

{% for jugador in site.data.jugadores %} 
    {% if jugadores.age < 30 %}
        {{ jugadores.name | upcase }} {{ jugadores.song }}
    {% endif %}
{% endfor %}

{% for rapero in site.data.raperos %} 
    {% if raperos.age > 30 %}
        {{ raperos.real_name}} {{ raperos.nba_song }} {{ raperos.artist_name }}
    {% endif %}
{% endfor %}
