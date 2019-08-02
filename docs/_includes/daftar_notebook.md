{%- assign base_link = site.data.site_config.nbviewer -%}
{%- assign github_link = site.data.site_config.github -%}
{%- assign raw_link = site.data.site_config.rawgithub -%}
{%- assign google_link = site.data.site_config.googlecolab -%}
{%- assign collection = include.source | reverse -%}
{%- for item in collection -%}
{% if item %}
-  **{{ item.title }}**<br><i class="fas fa-calendar-day"></i> `{{ item.date }}` \| <i class="fas fa-code-branch"></i> `{{ item.version }}` \| [<i class="fas fa-book-open"></i>]({{ base_link }}/notebook/{{ item.notebook }}.ipynb) \| [<i class="fab fa-github"></i>]({{ github_link }}/notebook/{{ item.notebook }}.ipynb) \| [<i class="fas fa-download"></i>]({{ raw_link }}/notebook/{{ item.notebook }}.ipynb) \| [<i class="fab fa-google"></i>]({{ google_link }}/notebook/{{ item.notebook }}.ipynb) \| [<i class="fas fa-user"></i>](https://github.com/{{ item.author }})
{%- endif -%}
{%- endfor -%}
