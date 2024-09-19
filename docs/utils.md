{%- macro tableSubItem(table, name, iucd) -%}
    {% if iucd is defined %}➡ _{{ table }}: {% endif %}{{ name }}{% if iucd is defined %}_{% endif %}
{%- endmacro -%}