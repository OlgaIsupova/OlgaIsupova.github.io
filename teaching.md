---
layout: default
title: Teaching
---

# Teaching

I am accepting new PhD and Masters students.

[//]: # (-- A fully-funded PhD position is available on [Unsupervised Outlier Detection](https://www.findaphd.com/phds/project/unsupervised-outlier-detection-for-high-dimensional-data/?p118345), supported by [UKRI Centre for Doctoral Training on Accountable, Responsible and Transparent AI](https://cdt-art-ai.ac.uk/). Deadline for application is **7 December 2020**)

[//]: # (-- A fully-funded PhD position is available on [Learning Disentangled Representations](https://www.findaphd.com/phds/project/learning-disentangled-representations-to-achieve-responsible-and-transparent-ai/?p126159), supported by [UKRI Centre for Doctoral Training on Accountable, Responsible and Transparent AI](https://cdt-art-ai.ac.uk/). Deadline for application is **7 December 2020**) 

-- A fully-funded PhD position is available on [Generative Modelling](https://www.findaphd.com/phds/project/deep-generative-modelling-from-classic-probabilistic-perspective/?p127707). Deadline for application is **21 February 2021**

**Courses:**
{% for course in site.data.teaching %}
* **{{ course.title}}** \\
  {{ course.role}} \\
  {{ course.where}}, {{ course.year}} 
  {% if course.links %} \\
    {% for link in course.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}

