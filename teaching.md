---
layout: default
title: Teaching
---

# Teaching

{% for course in site.data.teaching %}
* **{{ course.title}}** \\
  {{ course.role}} \\
  {{ course.where}}, {{ course.year}} 
  {% if course.links %} \\
    {% for link in course.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}

