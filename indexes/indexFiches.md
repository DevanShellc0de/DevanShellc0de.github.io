---
layout: default
permalink: /fiches/
title: Fiches
---
<p align="center">TOUTES LES FICHES</p>
<p align="center">Cette section centralise toutes les cheat sheet concernant Windows et Linux.</p><br>


 {% for post in site.tags.fiche %}
  <article>
  <div class="date"><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_string }}</time></div>
    <h2>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>

  </article>
{% endfor %}
