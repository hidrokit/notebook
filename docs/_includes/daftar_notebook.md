{%- assign base_link = site.data.site_config.nbviewer -%}
{% for item in include.source %}
- `{{ item.date }}|{{ item.version }}` [**[View on NBViewer]**{: .text-delta}]({{ base_link }}/notebook/{{ item.notebook }}.ipynb) {{ item.title }} oleh [{{ item.author }}](https://github.com/{{ item.author }}).
{%- endfor -%}
