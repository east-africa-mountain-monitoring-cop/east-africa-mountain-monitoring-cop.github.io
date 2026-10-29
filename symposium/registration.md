---
layout: default
title: Symposium registration
permalink: /symposium/registration/
---

<div class="page-header page-header--symposium">
  <div class="container">
    <p class="eyebrow">GEOMountain Symposium</p>
    <h1>Registration & Abstract submission</h1>
  </div>
</div>

<div class="container prose" markdown="1">

<p>Welcome! Use this page to register for the upcoming **GEOMountain Symposium**. The symposium is open to a maximum of 60 participants.  We invite academics, field researchers, policy stakeholders, local practitioners and students working on East African mountain environments to register.</p>

<p>There will is no registration fee. Lunch and coffee/tea breaks will be provided. Otherwise, participants are expected to fund themselves.</p>

**Financial support:**  

<p>A very limited number of grants is available for travel and subsistence and reserved for students/ junior academic researchers. These grants will be awarded on a competitive basis.</p>
<p>To apply for support, one must submit an abstract through the portal, including a paragraph ("motivation letter") to explain why you believe you should be supported, how the symposium / workshops will benefit from from your participation, and/or how your participation will benefit your home institution. Make sure to have this motivation letter ready and add it as part of your abstract before you start the registration.</p>

**Important dates:**

- **Abstract submission closes:** November 27, 2026
- **Registration closes:** December 24, 2027

{% if site.symposium_registration_url and site.symposium_registration_url != '' %}
<div class="cta-block">
  <p>Ready to join us? Use the link below to complete your symposium registration.</p>
  <a class="button" href="{{ site.symposium_registration_url }}" target="_blank" rel="noopener">Open registration form</a>
</div>
{% else %}
<div class="empty-state">
  <strong>Registration is not open yet.</strong>
  <p>When the form is ready, add its URL to <code>symposium_registration_url</code> in <code>_config.yml</code>.</p>
</div>
{% endif %}

<!-- <p>If you also wish to submit an abstract, please use the <a href="{{ '/symposium/abstracts/' | relative_url }}">abstract submission page</a>.</p> !-->

</div>
