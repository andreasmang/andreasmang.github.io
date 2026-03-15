---
layout: default
title: Publications
---

## Selected Publications

A more complete list of publications can be found on my [Google Scholar profile](https://scholar.google.com/citations?user=CJc0_msAAAAJ&hl=en).

{% for pub in site.data.publications %}
- {% if pub.authors and pub.authors.size > 0 %}{{ pub.authors }}, {% endif %}*{{ pub.title }}*.{% if pub.venue != "" %} {{ pub.venue }}.{% endif %}{% if pub.doi %} [doi]({{ pub.doi }}){% endif %}{% if pub.arxiv %} [arXiv]({{ pub.arxiv }}){% endif %} {% if pub.category == "bookchapter" %}<span class="pub-category bookchapter">chapter</span>{% elsif pub.category == "book" %}<span class="pub-category book">book</span>{% else %}<span class="pub-category {{ pub.category }}">{{ pub.category }}</span>{% endif %}
{% endfor %}
