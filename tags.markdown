---
layout: base
title: categories of stesselation
---
<div class="page-header">
  <h1>Posts by Tag</h1>
</div>

<div class="row">
  <div class="span14">

{% for cat in site.categories | sort %}
{% capture tag %}{{ cat | first }}{% endcapture %}
<a name="{{ tag }}">
</a>
<h2>{{ tag | replace:'_',' ' }}</h2>
<ul>
{% for post in site.categories[tag] %}
{% include postitem.markdown %}
{% endfor %}
</ul>
{% endfor %}

</div>
</div>
