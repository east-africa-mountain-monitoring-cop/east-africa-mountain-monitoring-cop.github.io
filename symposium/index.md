---
layout: default
title: GEOMountain Symposium in recognition of 30 years of collaboration between Swiss and Kenyan institutions under Global Atmopshere Watch (GAW)
permalink: /symposium/
---

<div class="page-header page-header--symposium">
  <div class="container">
    <p class="eyebrow">Activity</p>
    <h1>GEOMountain Symposium</h1>
    <p>A meeting space within the East Africa Community of Practice on Mountain Monitoring.</p>
    <div class="button-row">
      <a class="button" href="{{ '/symposium/program/' | relative_url }}">Programme</a>
      <a class="button button--secondary" href="{{ '/symposium/registration/' | relative_url }}">Registration</a>
      <a class="button button--secondary" href="{{ '/symposium/abstracts/' | relative_url }}">Abstract submission</a>
    </div>
  </div>
</div>

<div class="container prose" markdown="1">

## Symposium overview

The symposium will highlight the long collaboration between Kenya and Switzerland under the WMO Global Atmosphere Watch (GAW) program. It will also establish an "East Africa Community of Practice on Mountain Monitoring (EAMM CoP)" to foster collaboration of organizations working on related topics in the East Africa area.

<div class="callout">
  <h3>Important dates</h3>
  <p>Add confirmed deadlines here. Until then, this box can remain as a placeholder.</p>
</div>

## Themes

The symposium will place the initial EAMM CoP emphasis on the **Mount Kenya area**, **climate monitoring** and **atmospheric composition**, while leaving room for closely related mountain-observation topics, including water cycle, land-use, ecosystem research, etc.

## Co-Sponsors

We gratefully acknowledge the organizations supporting the GEOMountain Symposium. Their contributions help make the meeting possible and support collaboration, exchange and capacity development within the East Africa Community of Practice on Mountain Monitoring.

{% if site.data.sponsors and site.data.sponsors.size > 0 %}
<div class="logo-grid">
  {% for sponsor in site.data.sponsors %}
    <a class="logo-card" href="{{ sponsor.url }}" title="{{ sponsor.name }}">
      {% if sponsor.logo and sponsor.logo != '' %}
        <img src="{{ sponsor.logo | relative_url }}" alt="{{ sponsor.name }} logo">
      {% else %}
        <span>{{ sponsor.name }}</span>
      {% endif %}
    </a>
  {% endfor %}
</div>
{% else %}
<div class="empty-state">
  <p>Co-sponsor logos will be added here.</p>
</div>
{% endif %}

</div>
