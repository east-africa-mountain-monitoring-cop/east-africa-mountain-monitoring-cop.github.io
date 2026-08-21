---
layout: default
title: Symposium registration
permalink: /symposium/registration/
---

<div class="page-header page-header--symposium">
  <div class="container">
    <p class="eyebrow">GEOMountain Symposium</p>
    <h1>Registration</h1>
  </div>
</div>

<div class="container prose" markdown="1">
Add practical registration information here: eligibility, fees if any, deadlines, capacity, data-protection information and what participants should expect after registering.

{% if site.symposium_registration_url and site.symposium_registration_url != '' %}
<a class="button" href="{{ site.symposium_registration_url }}">Open registration form</a>
{% else %}
<div class="empty-state">
  <strong>Registration is not open yet.</strong>
  <p>When the form is ready, add its URL to <code>symposium_registration_url</code> in <code>_config.yml</code>.</p>
</div>
{% endif %}
</div>
