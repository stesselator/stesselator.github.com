{% if page.categories.size > 0 %}
to {% for cat in page.categories %}
<a href="/tags.html#{{ cat }}">{{ cat | replace:'_',' ' }}</a>{% if forloop.last == false %}, {% endif %}
{% endfor %}
{% endif %}
{% if post.categories.size > 0 %}
to {% for cat in post.categories %}
<a href="/tags.html#{{ cat }}">{{ cat | replace:'_',' ' }}</a>{% if forloop.last == false %}, {% endif %}
{% endfor %}
{% endif %}
