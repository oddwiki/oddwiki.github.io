{% if include.item.references %}
# References
{% for reference in include.item.references %}
  {{ reference }}
{% endfor %}
{% endif %}