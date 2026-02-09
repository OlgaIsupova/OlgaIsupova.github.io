---
layout: default
title: Publications and Code
---

# Publications and Code

## Highlighted Publications

### Elephant Detection from Satellite Imagery
I. Duporge*, **O. Isupova***, S. Reece, D. W. Macdonald, T. Wang. ``Using very high‐resolution satellite imagery and deep learning to detect 
and count African elephants in heterogeneous landscapes'' *Remote Sensing in Ecology and Conservation*, 2021  

**180+ citations Top cited/downloaded paper 2019-2020**  
📰 [BBC Coverage](https://www.bbc.co.uk/news/science-environment-55737086) | 📄 [Paper](https://zslpublications.onlinelibrary.wiley.com/doi/full/10.1002/rse2.195) | 💾 [Data](https://zenodo.org/records/17360762)

### Mining Environmental Risk Assessment
R. Balaniuk, **O. Isupova**, S. Reece

**Mining and tailings dam detection in satellite imagery using deep learning**  

Sensors, 2020  

**80+ citations Discovered 263 unregistered mines**  
📄 [Paper](https://www.mdpi.com/1424-8220/20/23/6936) | 💾 [Code](https://github.com/remis/mining-discovery-with-deep-learning)

### Crowdsourced Learning (Best Paper Award 🏆)
**O. Isupova**, Y. Li, D. Kuzin, S. J. Roberts, K. Willis, S. Reece 

**BCCNet: Bayesian classifier combination neural network**  

NeurIPS Workshop on ML for Developing World, 2018  

**Best Paper Award**  
📄 [Paper](https://arxiv.org/abs/1811.12258) | 💾 [Code](https://github.com/OlgaIsupova/BCCNet)

{% for year in site.data.papers %}
 <h2> {{ year.title}} </h2>
 {% for paper in year.papers %}
   * {{ paper.authors | array_to_sentence_string }}. 
     ``{{ paper.title}}'' 
     *{{ paper.where}}*
     {% if paper.links %} \\
       {% for link in paper.links %} [ {{ link.title}} ]({{link.url}}) {% endfor %}
     {% endif %}
   {% endfor %}
{% endfor %}
