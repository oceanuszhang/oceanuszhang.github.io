---
layout: page
title: Bookshelf
permalink: /books/
nav: true
nav_order: 10
---

Books I've especially loved are marked with a ★.

{% for year_entry in site.data.books.years %}

## {{ year_entry.year }}

{% if year_entry.books and year_entry.books.size > 0 %}
{% for book in year_entry.books %}
- {% if book.favorite %}★ {% endif %}*{{ book.title }}* — {{ book.author }}
{% endfor %}
{% else %}
*(coming soon)*
{% endif %}

{% endfor %}
