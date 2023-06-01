---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## 2023

- <span style="color:gray">[To be published]</span> Blivet et al. _Participation de l’équipe TTGV à DEFT 2023 : Réponse automatique à des QCM issus d’examens en pharmacie._ Actes de Atelier DÉfi Fouille de Textes (DEFT) (DEFT’2023).  
<span style="color:purple">*Keywords: multilabel classification, pre-trained models, health data*</span>

<!-- - <font color=gray> [To be published] </font>  F. Gaschi, I. El Baamrani, B. Gendron, P. Rastin, Y. Toussaint. _CoSwitchMap : Using Code-Switching to Learn an Unsupervised Bilingual Word Embedding._ Accepted for the 2023 Student Research Workshop of the Association for Computational Linguistics.  
<span style="color:darkblue">*Keywords: code-switching, word embeddings, multilingual alignment, unsupervised mapping.* </span> -->
