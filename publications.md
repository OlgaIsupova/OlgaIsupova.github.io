---
layout: default
title: Publications and Code
---

# Publications and Code

{% for year in site.data.papers %}
 <h2> {{ year.title}} </h2>
 {% for paper in year.papers %}
   * {{ paper.authors | array_to_sentence_string }} \\
     **{{ paper.title}}** \\
     {{ paper.where}} 
     {% if paper.achivements %} \\
       {% for achive in paper.achivements %} **{{ achive}}** {% endfor %}
     {% endif %}
     {% if paper.links %} \\
       {% for link in paper.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
     {% endif %}
   {% endfor %}
{% endfor %}
