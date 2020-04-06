---
title: Trapped Signal 📶
description: Tech and life in the age of COVID-19.
subtitle: Because we're frantically trying to maintain our families, jobs, and servers while stuck at home and there’s a zombie apocalypse outside.
layout: layouts/base.njk
---

{%- for page in collections.episode -%}
<a href="{{ page.url }}">
  <div>
    <h2>{{page.data.title}}</h2><time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <p>{{ page.data.guests }} discuss {{page.data.description}}</p>
  </div>
</a>
{%- endfor -%}
