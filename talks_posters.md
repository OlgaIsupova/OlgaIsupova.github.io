---
layout: default
title: Talks and Posters
---

# Talks and Posters

{% for talk in site.data.talks_posters %}
* **{{ talk.title}}** \\
  {{ talk.authors | array_to_sentence_string}} \\
  {{ talk.where}}, {{ talk.year}} 
  {% if talk.links %} \\
    {% for link in talk.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}

