---
layout: default
title: Publications
---

## Selected Publications

A more complete list of publications can be found on my [Google Scholar profile](https://scholar.google.com/citations?user=CJc0_msAAAAJ&hl=en).

### Preprints

{% for pub in site.data.publications %}{% if pub.category == "preprint" %}
- {{ pub.authors }}, *{{ pub.title }}*.{% if pub.doi %} [doi]({{ pub.doi }}){% endif %}{% if pub.arxiv %} [arXiv]({{ pub.arxiv }}){% endif %}
{% endif %}{% endfor %}

### Book Chapter

{% for pub in site.data.publications %}{% if pub.category == "book" %}
- {{ pub.authors }}, *{{ pub.title }}*. {{ pub.venue }}.{% if pub.doi %} [doi]({{ pub.doi }}){% endif %}{% if pub.arxiv %} [arXiv]({{ pub.arxiv }}){% endif %}
{% endif %}{% endfor %}

### Journal Articles

{% for pub in site.data.publications %}{% if pub.category == "journal" %}
- {{ pub.authors }}, *{{ pub.title }}*. {{ pub.venue }}.{% if pub.doi %} [doi]({{ pub.doi }}){% endif %}{% if pub.arxiv %} [arXiv]({{ pub.arxiv }}){% endif %}
{% endif %}{% endfor %}

### Conference Proceedings

{% for pub in site.data.publications %}{% if pub.category == "conference" %}
- {{ pub.authors }}, *{{ pub.title }}*. {{ pub.venue }}.{% if pub.doi %} [doi]({{ pub.doi }}){% endif %}{% if pub.arxiv %} [arXiv]({{ pub.arxiv }}){% endif %}
{% endif %}{% endfor %}
