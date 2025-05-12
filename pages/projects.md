---
layout: page-fullwidth          # gives us edge-to-edge space  :contentReference[oaicite:0]{index=0}
title:   ""
permalink: /projects/
header:
  title: Projects
  image_fullwidth: projects-header.png
---

<!-- ── HERO ────────────────────────────────────────────────────── -->
<section class="projects-hero">
  <h1>Portfolio Highlights</h1>
  <p class="lead">
    A selection of apps I’ve architected, prototyped, and developed.
  </p>
</section>


<!-- ── PROJECT GRID ────────────────────────────────────────────── -->
<ul class="projects-grid" data-equalizer>

{% assign projects = site.pages
     | where_exp:"p","p.categories contains 'projects'"
     | sort:"title" %}

{% for p in projects %}
  <li class="project-card" data-equalizer-watch>
    <a href="{{ p.url | relative_url }}">

      {% if p.image.thumb %}
        <img src="{{ p.image.thumb | relative_url }}"
             alt="{{ p.title }}">
      {% else %}
        <div class="thumb-placeholder">+</div>
      {% endif %}

      <h3>{{ p.title }}</h3>
      <p>{{ p.excerpt | strip_html | truncate: 120 }}</p>
      <span class="button tiny radius">Read&nbsp;More →</span>

    </a>
  </li>
{% endfor %}

</ul>
