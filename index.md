---
layout: index
---

**Welcome to OddWiki!**

This site is intended to become a fully-sourced Oddworld Encyclopedia, where
unsure fans can come to make sure their knowledge is correct.

<div id="cats">
{% for collection in site.collections %}
{% if collection.label %}
{% if collection.label != "posts" %}
<div class="category">
<h3>{{ collection.label }}</h3>
<ul>
{% for post in site[collection.label] %}
<li><a href="{{post.url}}">{{post.title}}</a></li>
{% endfor %}
</ul>
</div>
{% endif %}
{% endif %}
{% endfor %}
</div>
