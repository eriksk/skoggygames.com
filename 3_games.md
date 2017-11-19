---
layout: default
title: Games
permalink: /Games/
---

<h1>Games</h1>

<h2>Current Game Projects</h2>

<ul class="list-unstyled">
    <li><a href="http://puckoffgame.com/" target="_blank">Puck Off</a> - a local multiplayer hockey game.</li>
</ul>

<h2>Released Games</h2>

{% for game in site.data.games %}

<div class="row">
    <div class="twelve columns">
        <h3>
            <a href="{{ game.itchioGameUrl }}" target="_blank">
                {{ game.title }}
            </a>
        </h3>
        <i>{{ game.description }}</i> <br/>
        <iframe frameborder="0" src="https://itch.io/embed/{{ game.itchioGameId }}?border_width=0&amp;bg_color=ebebe0" width="208" height="165"></iframe>
    </div>
</div>

{% endfor %}
