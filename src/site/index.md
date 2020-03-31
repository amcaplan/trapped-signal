---
title: Trapped Signal 📶
subtitle: Because we're frantically trying to maintain our families, jobs, and servers while stuck at home and there’s a zombie apocalypse outside.
layout: layouts/base.njk
---

## We're all alone in this, together.

Life has changed for all of us, dramatically and at shocking speed.

We're all just trying to figure it out and make it to the next day.

And at the same time, we're all isolated from each other. Meetups and conferences are cancelled. Public social spaces are closed.

So how can we feel connected to a broader community?

It starts by remembering that our burden is shared. Every one of us is struggling with many things in our new (hopefully very temporary) reality.

So let's acknowledge it. Let's talk about it. Let's hear from other people who are in the same boat. Let's offer each other strength.

<p>We can do this.</p>


{%- for page in collections.post -%}
<a href="{{ page.url }}">
  <div>
    <h2>Episode {{ loop.index }}: {{page.data.title}}</h2><time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
    <p>{{page.data.description}}</p>
  </div>
</a>
{%- endfor -%}
