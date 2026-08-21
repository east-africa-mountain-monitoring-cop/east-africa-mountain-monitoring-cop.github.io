---
layout: default
title: Symposium programme
permalink: /symposium/program/
---

<div class="page-header page-header--symposium">
  <div class="container">
    <p class="eyebrow">GEOMountain Symposium</p>
    <h1>Programme</h1>
  </div>
</div>

<div class="container section">
{% if site.data.program and site.data.program.size > 0 %}
  {% for day in site.data.program %}
    <section class="program-day">
      <div class="program-day__heading">
        <h2>{{ day.day }}</h2>
        {% if day.date %}<span>{{ day.date | date: "%A, %-d %B %Y" }}</span>{% endif %}
      </div>

      <div class="program-list">
      {% for item in day.items %}
        <article class="program-item">
          <div class="program-time">
            <strong>{{ item.time }}</strong>
            {% if item.end %}<span>– {{ item.end }}</span>{% endif %}
          </div>
          <div>
            <h3>{{ item.title }}</h3>
            {% if item.speaker and item.speaker != '' %}<p class="meta">{{ item.speaker }}</p>{% endif %}
            {% if item.location and item.location != '' %}<p class="meta">{{ item.location }}</p>{% endif %}
            {% if item.description and item.description != '' %}<p>{{ item.description }}</p>{% endif %}
          </div>
        </article>
      {% endfor %}
      </div>
    </section>
  {% endfor %}
{% else %}
  <div class="empty-state">
    <h2>Programme in preparation</h2>
    <p>The programme will be published here. It can be maintained directly on GitHub by editing <code>_data/program.yml</code>.</p>
  </div>
{% endif %}
</div>
