# {{ include.item.name }}
{:.no_toc}

{% include building_blocks/wiki-notice.md %}

{% include building_blocks/quote.md %}

{% include toc.html %}

{{ include.item.summary }}

{% if include.item.gameplay %}
# Gameplay
{{ include.item.gameplay }}
{% endif %}

{% if include.item.story %}
# Story
{{ include.item.story }}
{% endif %}

{% include building_blocks/trivia.md %}

{% include building_blocks/gallery.md %}

{% include building_blocks/references.md %}
