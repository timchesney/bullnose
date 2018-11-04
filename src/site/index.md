---
title: Bullnose
subtitle: NZ couple resotring a historic building
layout: layouts/base.njk
---


<div class="posts">
{%- for page in collections.post | reverse -%}
  <h2>
    <a href="{{ page.url }}">{{ page.data.title }}</a>
  </h2>
  <time datetime="{{ page.date }}">{{ page.date | dateDisplay }}</time>
  <p>{{ page.data.subtitle}}</p>
{%- endfor -%}
</div>
