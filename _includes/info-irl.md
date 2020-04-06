# {{ include.item.name }}

> {{ include.item.quote }}

{{ include.item.summary }}

{% include toc.html %}

# Trivia
{{ include.item.trivia }}

# Gallery
{% for image in include.item.gallery %}
  ![]({{ image.image-url }})

  {{ image.description }}
{% endfor %}

# References
{% for reference in include.item.references %}
  * {{ reference }}
{% endfor %}
