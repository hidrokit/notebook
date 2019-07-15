{%- assign base_link = site.data.site_config.nbviewer -%}
{%- assign collection = include.source | reverse -%}
{%- for item in collection -%}
{% if item %}
- `{{ item.date }}|{{ item.version }}` [**[View on NBViewer]**{: .text-delta}]({{ base_link }}/notebook/{{ item.notebook }}.ipynb)<br>**{{ item.title }}** oleh [{{ item.author }}](https://github.com/{{ item.author }}).
{%- endif -%}
{%- endfor -%}
