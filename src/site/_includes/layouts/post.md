---
layout: layouts/base.njk
pageClass: posts
templateEngineOverride: njk, md
---

<h1>{{ title }}</h1>
{%- if subtitle %}<p class="subtitle">{{ subtitle }}</p>{% endif %}

<p class="date">
  Posted on <time datetime="{{ date }}">{{ date | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
  <div class="footnote">
    <p>
      This page is part of the posts section.
    </p>
  </div>
</main>
