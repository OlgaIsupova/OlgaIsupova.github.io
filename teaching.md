---
layout: default
title: Teaching
---

# Teaching

I am accepting new PhD and Master students.

-- A fully-funded (UK and EU) PhD position is available on [Unsupervised Outlier Detection](https://www.findaphd.com/phds/project/unsupervised-outlier-detection-for-high-dimensional-data/?p118345), supported by [UKRI Centre for Doctoral Training on Accountable, Responsible and Transparent AI](http://www.bath.ac.uk/centres-for-doctoral-training/ukri-centre-for-doctoral-training-in-accountable-responsible-and-transparent-ai/?fbclid=IwAR3evl5ZTPDJriVSrcy4n-53uVx5ST3bDgCntUQ7xpCnkHS49CboCx1hWBE). Deadline for application is **6 April 2020**

-- A fully-funded (UK and EU) PhD position is available on [Generative Modelling](https://www.findaphd.com/phds/project/deep-generative-modelling-from-the-classic-probabilistic-perspective/?p120065). Deadline for application is **29 March 2020**

**Courses:**
{% for course in site.data.teaching %}
* **{{ course.title}}** \\
  {{ course.role}} \\
  {{ course.where}}, {{ course.year}} 
  {% if course.links %} \\
    {% for link in course.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}

