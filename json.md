---
layout: page
title: Implementacion de Json
description: Json con jugadores y raperos
featured_image: json.jpg
---

{% for jugador in site.data.jugadores %} 
    {% if jugador.age < 30 %}
        {{ jugador.name | upcase }} {{ jugador.song }}
    {% endif %}
{% endfor %}

{% for rapero in site.data.raperos %} 
    {% if rapero.age > 30 %}
        {{ rapero.real_name }} {{ rapero.nba_song }} {{ rapero.artist_name }}
    {% endif %}
{% endfor %}
