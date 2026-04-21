---
layout: page
title: Awards
permalink: /awards/
description: Scholarships, fellowships, and academic honors.
nav: false
nav_order: 7
---

{% for award in site.data.awards.awards %}

<div style="margin-bottom: 2rem;">
  <h3 style="margin-bottom: 0.2rem;">{{ award.title }}</h3>
  <p style="color: var(--global-text-color-light); margin-bottom: 0.4rem;">
    {% if award.organization_url %}
      <a href="{{ award.organization_url }}" target="_blank">{{ award.organization }}</a>
    {% else %}
      {{ award.organization }}
    {% endif %}
    &nbsp;·&nbsp; {{ award.date }}
    {% if award.amount %}&nbsp;·&nbsp; <strong>{{ award.amount }}</strong>{% endif %}
  </p>
  <p>{{ award.description }}</p>
</div>

{% endfor %}
