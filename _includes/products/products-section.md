{% assign products = include.products | sort: "info.name" %}

<h2>{{ include.title | default: "Products" }}</h2>

{% if include.all-url %}
<div>
    <a href="{{include.all-url}}">View all</a>
</div>
{% endif %}

{% include kankoda/grids/grid.html items=products type="icons" %}