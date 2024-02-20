<h2>{{ include.title | default: "Products" }}</h2>
{% include kankoda/grids/grid.html items=include.products type="icons" %}