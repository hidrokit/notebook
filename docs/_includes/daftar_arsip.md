{%- assign base_link = site.data.site_config.nbviewer -%}
{% for item in site.data.archive %}
1. [{{ item.name }}]({{ base_link }}/{{ item.folder }}/{{ item.notebook }}.ipynb): {{ item.description }}
{%- endfor -%}
