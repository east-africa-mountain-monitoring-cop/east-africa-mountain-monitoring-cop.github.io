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

        {% if item.type == "parallel" %}
          <article class="program-item program-item--parallel">
            <div class="program-time">
              <strong>{{ item.time }}</strong>
              {% if item.end %}<span>– {{ item.end }}</span>{% endif %}
            </div>

            <div class="parallel-block">
              {% if item.title and item.title != '' %}
                <h3 class="parallel-block__title">{{ item.title }}</h3>
              {% endif %}

              <div class="parallel-tracks">
                {% for track in item.tracks %}
                  <section class="parallel-track">
                    <header class="parallel-track__header">
                      {% if track.name and track.name != '' %}
                        <p class="parallel-track__label">{{ track.name }}</p>
                      {% endif %}

                      {% if track.title and track.title != '' %}
                        <h3>{{ track.title }}</h3>
                      {% endif %}

                      {% if track.location and track.location != '' %}
                        <p class="meta">{{ track.location }}</p>
                      {% endif %}

                      {% if track.chair and track.chair != '' %}
                        <p class="parallel-track__detail"><strong>Chair:</strong> {{ track.chair }}</p>
                      {% endif %}

                      {% if track.description and track.description != '' %}
                        <p>{{ track.description }}</p>
                      {% endif %}
                    </header>

                    {% if track.items and track.items.size > 0 %}
                      <div class="parallel-track__timeline">
                        {% for track_item in track.items %}
                          <article class="parallel-track__item">
                            <div class="parallel-track__time">
                              <strong>{{ track_item.time }}</strong>
                              {% if track_item.end %}<span>– {{ track_item.end }}</span>{% endif %}
                            </div>

                            <div class="parallel-track__content">
                              <h4>{{ track_item.title }}</h4>

                              {% if track_item.speaker and track_item.speaker != '' %}
                                <p class="meta">{{ track_item.speaker }}</p>
                              {% endif %}

                              {% if track_item.location and track_item.location != '' %}
                                <p class="meta">{{ track_item.location }}</p>
                              {% endif %}

                              {% if track_item.description and track_item.description != '' %}
                                <p>{{ track_item.description }}</p>
                              {% endif %}
                            </div>
                          </article>
                        {% endfor %}
                      </div>
                    {% endif %}
                  </section>
                {% endfor %}
              </div>
            </div>
          </article>

        {% else %}
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
        {% endif %}

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
