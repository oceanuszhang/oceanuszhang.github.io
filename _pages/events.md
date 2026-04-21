---
layout: page
title: Events
permalink: /events/
description: Talks, presentations, and conference participation.
nav: false
nav_order: 5
---

## Talks & Presentations

<div class="table-responsive">
<table class="table table-sm">
  <thead>
    <tr>
      <th>Talk</th>
      <th>Venue</th>
      <th>Location</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    {% for talk in site.data.events.presentations %}
    <tr>
      <td><em>{{ talk.title }}</em></td>
      <td>{{ talk.event }}</td>
      <td>{{ talk.location }}</td>
      <td>{{ talk.date }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
</div>

---

## Conference Participation

<div class="table-responsive">
<table class="table table-sm">
  <thead>
    <tr>
      <th>Conference</th>
      <th>Paper / Abstract</th>
      <th>Role</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    {% for conf in site.data.events.conferences %}
    <tr>
      <td>
        <strong>{{ conf.name }}</strong>{% if conf.location %}<br><small>{{ conf.location }}</small>{% endif %}
      </td>
      <td><em>{{ conf.paper }}</em></td>
      <td><span class="badge badge-primary">{{ conf.note }}</span><br>{{ conf.role }}</td>
      <td>{{ conf.date }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
</div>
