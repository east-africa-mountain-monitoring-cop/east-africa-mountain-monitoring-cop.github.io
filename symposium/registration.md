---
layout: default
title: Symposium registration
permalink: /symposium/registration/
---

<div class="page-header page-header--symposium">
  <div class="container">
    <p class="eyebrow">GEOMountain Symposium</p>
    <h1>CALL FOR ABSTRACTS</h1>
  </div>
</div>

<div class="container prose" markdown="1">
### Registration Overview

Welcome !Use this page to register for the upcoming  **GEOMountain Symposium**

**Eligibility:** 
Open to academics,field researchers,policy stakeholders,local practictioners and students working on  East African mountain environments.

**Registration** 
Standard Delegate **$1050 USD** | Student Rate:**$275 USD** *(Institutional ID required)* .

**Financial Support:** 
A limited number of travel grants and registration fee waivers
available

**IMPORTANT DEADLINES:**

**Abstract Submission Deadline:** December 13, 2026.

**Early Bird Registration Closes:**Deember 1,2026.

**Final Registration Deadline:**  Jananuary 20,2027.

**DATA PROTECTION POLICY:** 
All submitted details are handled securely  in  accordance with  standard privacy guidelines and will only be used for symposium communication.

**Upon submitting your form,you will receive an notification in less than a month  after carefully reviewing your abstract by the science committee.**

## Complete the Registration form and submit your Abstract.
{% if site.symposium_registration_url and site.symposium_registration_url != '' %}
<div class="cta-block">
  <p>Ready to join us?Click below  link to complete your registration  and abstract submission</p>
  <a class="button" href="{{ site.symposium_registration_url }}" target="_blank" rel="noopener">Open registration form</a>
</div>
{% else %}
<div class="empty-state">
  <strong>Registration form/Abstract submission</strong>
  <div class="form-embed-wrap">
    <iframe class="google-form-iframe" title="GEOMountain Symposium registration form" src="https://docs.google.com/forms/d/e/1FAIpQLScyCnqf-l1whtEzzIMwdY3q1Z2tUEN2Q5w8PDN9FZChZCBJrA/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
  </div>
  <p>When the form is ready, add its URL to <code>symposium_registration_url</code> in <code>_config.yml</code>.</p>
</div>
{% endif %}
</div>

