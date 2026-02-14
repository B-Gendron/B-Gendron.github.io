---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

{% include base_path %}

{% for post in site.softwares %}
  <div>
    <img src="../images/zss-logo-2.png" style="width:80%;">
  </div>
  {% include archive-single.html type="grid" %}
{% endfor %}

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