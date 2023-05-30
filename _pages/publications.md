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

- <span style="color:gray">[To be published]</span> Blivet et al Participation de l’équipe TTGV à DEFT 2023 : Réponse automatique à des QCM issus d’examens en pharmacie. Actes de Atelier DÉfi Fouille de Textes (DEFT) (DEFT’2023).  
      _Keywords: multilabel classification, pre-trained models, health data_

<!-- - <font color=gray> [To be published] </font>  F. Gaschi, I. El Baamrani, B. Gendron, P. Rastin, Y. Toussaint. CoSwitchMap : Using Code-Switching to Learn an Unsupervised Bilingual Word Embedding. Submitted to 2023 Student Research Workshop of the Association for Computational Linguistics.
      _Keywords: code-switching, word embeddings, multilingual alignment, unsupervised mapping._ -->
