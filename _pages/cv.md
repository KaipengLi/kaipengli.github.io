---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 5
description: Download my curriculum vitae.
---

{% assign uploaded_cv = site.static_files | where: "path", "/assets/pdf/cv.pdf" | first %}

{% if uploaded_cv %}

<p>
  <a class="btn btn-sm z-depth-0" href="{{ '/assets/pdf/cv.pdf' | relative_url }}" target="_blank" rel="noopener">Download CV</a>
</p>

<object data="{{ '/assets/pdf/cv.pdf' | relative_url }}" type="application/pdf" width="100%" height="900">
  <p><a href="{{ '/assets/pdf/cv.pdf' | relative_url }}" target="_blank" rel="noopener">Open CV PDF</a></p>
</object>

{% else %}

CV PDF will be available soon.

{% endif %}
