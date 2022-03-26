{%- assign nbv_repo = site.data.site_config.nbviewer -%}
{%- assign nbv_base = site.data.site_config.nbviewer_base -%}
{%- assign raw_link = site.data.site_config.rawgithub -%}
{%- assign github_link = site.data.site_config.github -%}
{%- assign gist_link = site.data.site_config.gist_url -%}

{%- assign collection = include.source -%}
{%- for item in collection -%}
<!-- CONDITIONAL IF GIST USED -->
{%- if item.gist -%}
<!-- IF GIST NOT EMPTY / TRUE -->
{%- capture nbv_link -%}
{{ nbv_base }}/gist/{{ item.gist_id }}
{%- endcapture -%}
{%- capture gh_link -%}
{{ gist_link }}/{{ item.gist_id }}
{%- endcapture -%}
{%- elsif item.folder != empty -%}
<!-- IF FOLDER NOT EMPTY -->
{%- capture nbv_link -%}
{{ nbv_repo }}/{{ item.folder }}/{{ item.notebook }}.ipynb
{%- endcapture -%}
{%- capture gh_link -%}
{{ github_link }}/{{ item.folder }}/{{ item.notebook }}.ipynb
{%- endcapture -%}
{%- endif -%}

{%- if item.description -%}
{%- capture desc -%}
_{{ item.description }}_{: .text-epsilon}<br>
{%- endcapture -%}
{%- endif -%}

{%- if item.folder -%}
{%- capture dl_link -%}
<a href="{{ raw_link }}/{{ item.folder }}/{{ item.notebook }}.ipynb" download="{{ item.notebook }}.ipynb" target="_blank"><i class="fas fa-download"></i></a>
{%- endcapture -%}
{%- endif -%}

{%- if item.pdf -%}
{%- capture pdf_link -%}
<a href="{{ item.pdf }}" download="{{ item.notebook }}.pdf"><i class="far fa-file-pdf"></i></a> \| 
{%- endcapture -%}
{%- endif -%}

{% if item %}
- **{{ item.title }}** {{ dl_link }}<br>{{ desc }}
<i class="fas fa-calendar-day"></i> _{{ item.date | date: "%d %b %Y" }}_{: .text-delta} \| 
<i class="fas fa-code-branch"></i> _{{ item.version }}_{: .text-delta} \| 
[<i class="fas fa-book-open"></i>]({{ nbv_link }}) \|
[<i class="fab fa-github"></i>]({{ gh_link }}) \| {{ pdf_link }}
[@{{ item.author }}](https://github.com/{{ item.author }}){: .text-delta}
{%- endif -%}

{%- assign desc = nil -%}
{%- assign dl_link = nil -%}
{%- assign pdf_link = nil -%}

{%- endfor -%}

