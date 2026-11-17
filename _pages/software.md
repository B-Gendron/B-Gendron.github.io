---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

{% include base_path %}

<style>
.sw-intro { margin: 0 0 1.5em; color: #555; }

.sw-list { margin: 0; padding: 0; list-style: none; border-top: 1px solid #e3e6ea; }
.sw-item {
  display: grid;
  grid-template-columns: 120px minmax(0, 1fr);
  gap: 1.5em;
  align-items: start;
  margin: 0;
  padding: 1.6em 0;
  border-bottom: 1px solid #e3e6ea;
}
.sw-logo {
  display: flex; align-items: center; justify-content: center;
  width: 120px; height: 120px; padding: 10px;
  border: 1px solid #e3e6ea; border-radius: 8px; background: #fff;
}
.sw-logo img { max-width: 100%; max-height: 100%; object-fit: contain; }

.sw-body h2 { margin: 0 0 0.15em; padding: 0; border: 0; font-size: 1.25em; }
.sw-body h2 a { color: inherit; text-decoration: none; }
.sw-body h2 a:hover { text-decoration: underline; }
.sw-meta { margin: 0 0 0.6em; font-size: 0.8em; color: #777; }
.sw-desc { margin: 0 0 0.8em; font-size: 0.95em; line-height: 1.5; }

.sw-links { display: flex; flex-wrap: wrap; gap: 0.5em; }
.sw-links a {
  display: inline-block; padding: 0.35em 0.9em;
  border: 1px solid #ccd3dc; border-radius: 6px;
  font-size: 0.85em; color: #333; text-decoration: none;
}
.sw-links a:hover { border-color: #6c91bf; color: #000; }
.sw-links a.sw-primary { background: #333; border-color: #333; color: #fff; }
.sw-links a.sw-primary:hover { background: #000; }

@media (max-width: 600px) {
  .sw-item { grid-template-columns: 72px minmax(0, 1fr); gap: 1em; }
  .sw-logo { width: 72px; height: 72px; padding: 6px; }
}
</style>

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
