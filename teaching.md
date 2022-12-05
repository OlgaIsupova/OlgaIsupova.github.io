---
layout: default
title: Teaching
---

# Teaching

I am accepting new PhD and Masters students.

[//]: # (-- A fully-funded PhD position is available on [Unsupervised Outlier Detection](https://www.findaphd.com/phds/project/unsupervised-outlier-detection-for-high-dimensional-data/?p118345), supported by [UKRI Centre for Doctoral Training on Accountable, Responsible and Transparent AI](https://cdt-art-ai.ac.uk/). Deadline for application is **7 December 2020**)

-- A fully-funded PhD position is available on [Learning Disentangled Representations](https://www.findaphd.com/phds/project/learning-disentangled-representations-to-achieve-responsible-and-transparent-ai/?p126159), supported by [UKRI Centre for Doctoral Training on Accountable, Responsible and Transparent AI](https://cdt-art-ai.ac.uk/). 

-- A fully-funded (home student fees) PhD position is available on [Generative Modelling](https://www.findaphd.com/phds/project/deep-generative-modelling-from-classic-probabilistic-perspective/?p151169). Deadline for application is **22 January 2023**

-- A fully-funded PhD position is available on [Finding Biomarkers for Alzheimer’s disease](https://www.findaphd.com/phds/project/epsrc-dtp-phd-project-artificial-intelligence-enabled-identification-of-potential-immune-biomarkers-in-cognitive-decline-decode/?p151778). Deadline for application is **5 February 2023**

**Courses:**
{% for course in site.data.teaching %}
* **{{ course.title}}** \\
  {{ course.role}} \\
  {{ course.where}}, {{ course.year}} 
  {% if course.links %} \\
    {% for link in course.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}

