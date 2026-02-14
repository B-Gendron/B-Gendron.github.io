---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

{% include base_path %}

<div class="software-grid">
{% for post in site.softwares %}
  <a href="{{ post.url | relative_url }}" class="software-card">
    
    <img src="/images/zss-logo-2.png" alt="{{ post.title }}">

    <h3>{{ post.title }}</h3>
    <p>{{ post.excerpt }}</p>

  </a>
{% endfor %}
</div>


<!-- ---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

## [ZSS: Zotero Similarity Selection](https://B-Gendron.github.io/softwares/software-1/)

<div>
<img src="../images/zss-logo-2.png" style="width60%;">
</div> -->