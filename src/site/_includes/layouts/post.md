---
layout: layouts/base.njk
pageClass: posts
templateEngineOverride: njk, md
---

<p class="date">
  Posted on <time datetime="{{ date }}">{{ date | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
  {{ guests }} discuss {{description}}
  <iframe src="https://anchor.fm/trapped-signal/embed/episodes/{{ anchorLink}}" height="102px" width="100%" frameborder="0" scrolling="no"></iframe>

  <div class="footnote">
    <p>
      <a href="/">Back to All Episodes</a>
    </p>
  </div>
</main>
