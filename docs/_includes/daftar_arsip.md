{%- assign base_link = site.data.site_config.nbviewer -%}
{%- assign sorted = (site.data.archive | sort: 'date') | reverse -%}
{% for item in sorted %}
- `{{ item.date }}|{{ item.version }}` [**[View on NBViewer]**{: .text-delta}]({{ base_link }}/{{ item.folder }}/{{ item.notebook }}.ipynb)<br>{{ item.title }} oleh [{{ item.author }}](https://github.com/{{ item.author }}).
{%- endfor -%}
