---
---

# Index

{% for collection in site.collections %}
<section>
<h1>{{ collection.label }}</h1>

{% for post in site.[collection.label] %}
<a href="{{post.url}}">{{post.title}}</a>
{% endfor %}

</section>
{% endfor %}
