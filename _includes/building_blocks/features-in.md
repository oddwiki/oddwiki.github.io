{% if include.item.features-in %}
# Features In
{% for game in include.item.features-in %}
  * {{ game }}
{% endfor %}
{% endif %}