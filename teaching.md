---
layout: default
title: Teaching
---

# Teaching

I am accepting new PhD students.

* A fully-funded (UK and EU) PhD position is available on [Unsupervised Outlier Detection](https://www.findaphd.com/phds/project/unsupervised-outlier-detection-for-high-dimensional-data/?p118345), supported by [UKRI Centre for Doctoral Training on Accountable, Responsible and Transparent AI](http://www.bath.ac.uk/centres-for-doctoral-training/ukri-centre-for-doctoral-training-in-accountable-responsible-and-transparent-ai/?fbclid=IwAR3evl5ZTPDJriVSrcy4n-53uVx5ST3bDgCntUQ7xpCnkHS49CboCx1hWBE). Deadline for application is **10 February 2020**

{% for course in site.data.teaching %}
* **{{ course.title}}** \\
  {{ course.role}} \\
  {{ course.where}}, {{ course.year}} 
  {% if course.links %} \\
    {% for link in course.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
  {% endif %}
{% endfor %}

