---
layout: default
title: Abstract submission
permalink: /symposium/abstracts/
---

<div class="page-header page-header--symposium">
  <div class="container">
    <p class="eyebrow">GEOMountain Symposium</p>
    <h1>Abstract submission</h1>
  </div>
</div>

<div class="container prose" markdown="1">
Use this page for the call for abstracts, themes, submission deadline, abstract length, oral/poster preference, review process and publication conditions.

A structured web form is recommended instead of document uploads. Suggested fields include title, corresponding author, affiliation, co-authors, abstract text, keywords, topic/session and oral/poster preference.

{% if site.symposium_abstract_url and site.symposium_abstract_url != '' %}
<a class="button" href="{{ site.symposium_abstract_url }}">Submit an abstract</a>
{% else %}
<div class="empty-state">
  <strong>Abstract submission is not open yet.</strong>
  <p>When the form is ready, add its URL to <code>symposium_abstract_url</code> in <code>_config.yml</code>.</p>
</div>
{% endif %}
</div>
