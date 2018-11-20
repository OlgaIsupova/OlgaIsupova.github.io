---
layout: default
title: Publications and Code
---

# Publications and Code

{% for year in site.data.papers %}
 ## {{ year.title}}
 {% for paper in year.papers %}
 * {{ paper.authors | array_to_sentence_string }} \\
   **{{ paper.title}}** \\
   {{ paper.where}} 
   {% if paper.links %} \\
     {% for link in paper.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
   {% endif %}
 {% endfor %}
{% endfor %}
