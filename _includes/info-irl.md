# {{ include.item.name }}
{:.no_toc}

> {{ include.item.quote }}

{% include toc.html %}

{{ include.item.summary }}

# Trivia
{% for trivia in include.item.trivia %}
  * {{ trivia }}
{% endfor %}

# Gallery
{% for image in include.item.gallery %}
  {% include figure.html url=image.image-url text=image.description %}
{% endfor %}

# References
{% for reference in include.item.references %}
  * {{ reference }}
{% endfor %}
