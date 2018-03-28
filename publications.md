---
layout: default
title: {Publications and Code}
---

# Publications

{% for paper in site.data.papers %}
* {{ paper.authors | array_to_sentence_string }} \\
  **{{ paper.title}}** \\
  {{ paper.where}}, {{ paper.year}} 
  {% if paper.links %} \\
    {% for link in paper.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}
