# {{ include.item.name }}

> {{ include.item.quote }}

{{ include.item.summary }}

{% include toc.html %}

# Appearance
{{ include.item.appearance }}

# Personality
{{ include.item.personality }}

# Appears In
{% for appearance in include.item.appears-in %}
  * {{ appearance }}
{% endfor %}

# Trivia
{{ include.item.trivia }}

# Gallery
{% for image in include.item.gallery %}
  {% include figure.html url=image.image-url text=image.description %}
{% endfor %}

# References
{% for reference in include.item.references %}
  {{ reference }}
{% endfor %}
