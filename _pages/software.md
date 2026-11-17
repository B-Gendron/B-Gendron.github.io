---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

{% include base_path %}

<p class="sw-intro">Tools I developed for my research and made available to others. Each one has a page explaining what it does and how to use it.</p>

{% assign softwares = site.softwares | sort: "order" %}
<ul class="sw-list">
{% for sw in softwares %}
  <li class="sw-item">
    <a class="sw-logo" href="{{ sw.url | relative_url }}" aria-hidden="true" tabindex="-1">
      <img src="{{ sw.logo | relative_url }}" alt="">
    </a>
    <div class="sw-body">
      <h2><a href="{{ sw.url | relative_url }}">{{ sw.title }}</a></h2>
      {% if sw.meta %}<p class="sw-meta">{{ sw.meta }}</p>{% endif %}
      <p class="sw-desc">{{ sw.excerpt | strip_html }}</p>
      <div class="sw-links">
        <a class="sw-primary" href="{{ sw.url | relative_url }}">Read the guide</a>
        {% if sw.github %}<a href="{{ sw.github }}" target="_blank" rel="noopener">GitHub</a>{% endif %}
      </div>
    </div>
  </li>
{% endfor %}
</ul>
