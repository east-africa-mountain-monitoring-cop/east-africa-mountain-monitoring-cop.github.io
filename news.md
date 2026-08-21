---
layout: default
title: News
permalink: /news/
---

<div class="page-header">
  <div class="container">
    <p class="eyebrow">Updates</p>
    <h1>News</h1>
    <p>Announcements, meeting updates and other developments from the Community of Practice.</p>
  </div>
</div>

<div class="container section">
{% if site.posts.size > 0 %}
  <div class="news-list">
  {% for post in site.posts %}
    <article class="news-item">
      <p class="meta">{{ post.date | date: "%-d %B %Y" }}</p>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt | strip_html | truncate: 260 }}</p>
      <a class="text-link" href="{{ post.url | relative_url }}">Read more →</a>
    </article>
  {% endfor %}
  </div>
{% else %}
  <div class="empty-state">
    <p>No news has been published yet.</p>
  </div>
{% endif %}

{% if site.wiki_url and site.wiki_url != '' %}
  <div class="callout">
    <h2>Working information and community knowledge</h2>
    <p>The GitHub wiki can be used for evolving notes, meeting material, technical information and other collaborative content that does not need to be a formal website page.</p>
    <a class="button button--outline" href="{{ site.wiki_url }}">Open the wiki</a>
  </div>
{% endif %}
</div>
