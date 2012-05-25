---
layout: base
title: "Flirting with the Critics"
---
<div class="page-header">
  <h1>The Stesselator Blog</h1>
  <small>Flirting with the Metro riders.  They know they like it.</small>
</div>

<div class="row">
  <div class="span14">

{% for post in site.posts offset: 0 limit: 10 %}
<h2><a href='{{ post.id }}.html'>{{ post.title }}</a></h2>
<span id="date">Posted {{ post.date | date_to_string }}{% include tags.markdown %}and has <a href="{{ post.id }}.html#disqus_thread">Comments</a></span>
  <div class="post">
  {{ post.content }}
  </div>
{% endfor %}

  </div>
</div>
