---
title: "Database & Data Mining Lab - Publications"
layout: gridlay
excerpt: "Database & Data Mining Lab - Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

<ul style="overflow: hidden">
  <li>We have published six papers (3 SIGMOD, 2 VLDB, 1 ICDE) in top database conferences in 2021</li>
  <li>We have published five papers (1 SIGMOD, 4 VLDB) in top database conferences in 2020</li>
  <li>We have published six papers (4 SIGMOD, 1 VLDB, 1 ICDE) in top database conferences in 2024</li>
</ul>

## Notice for undergrads 
For undergrads who are interested in big data, data management, and database systems, note that SIGMOD, VLDB, and ICDE are flagship conferences in these fields. We have published a lot of strong papers in these venues. We are competing with top universities worldwide, and actively seek for self-motivated students who would like to share our vision.

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

{% assign year_until = 2012%}

## International Journals
{% assign var_year = 2030 %}
{% for publi in site.data.publications.international_journals %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.month }} {{ publi.year}}
  {% if publi.ISSN != null %} (ISSN: {{publi.ISSN}}){% endif %} {% if publi.is_corresponding_author == true %} (Corresponding Author){% endif %} {% if publi.is_co-corresponding_author == true %} (Co-Corresponding Author){% endif %} {% if publi.link != null %} <a href="{{ publi.link }}">[PDF]</a> {% endif %} {% if publi.endmsg != null %} **{{ publi.endmsg }}** <br /> {% endif %}

{% endfor %}

## International Conference Proceedings
{% assign var_year = 2030 %}
{% for publi in site.data.publications.international_conference_proceedings %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.month }} {{ publi.year }}
  {% if publi.is_demo == true %} (Demo){% endif %} {% if publi.ISSN != null %} (ISSN: {{publi.ISSN}}){% endif %} {% if publi.is_corresponding_author == true %} (Corresponding Author){% endif %} {% if publi.is_co-corresponding_author == true %} (Co-Corresponding Author){% endif %} {% if publi.link != null %}<a href="{{ publi.link }}">[PDF]</a>{% endif %}{% if publi.ppt != null %}<a href="{{ publi.ppt }}">[PPT]</a>{% endif %} {% if publi.endmsg != null %}  **{{ publi.endmsg }}** <br /> {% endif %}

{% endfor %}

## Others
{% assign var_year = 2030 %}
{% for publi in site.data.publications.others %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.month }} {{ publi.year }} {% if publi.link != null %}
  <a href="{{ publi.link }}">[PDF]</a>
  {% endif %}

{% endfor %}

## Domestic Journals
{% assign var_year = 2030 %}
{% for publi in site.data.publications.domestic_journals %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.year }}년 {{ publi.month }}월 {% if publi.link != null %}
  <a href="{{ publi.link }}">[PDF]</a>
  {% endif %}

{% endfor %}


## Domestic Conference Proceedings
{% assign var_year = 2030 %}
{% for publi in site.data.publications.domestic_conference_proceedings %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.year }}년 {{ publi.month }}월 {% if publi.link != null %}
  <a href="{{ publi.link }}">[PDF]</a>
  {% endif %}

{% endfor %}

## International Patents
{% assign var_year = 2030 %}
{% for publi in site.data.publications.international_patents %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.month }} {{ publi.year }} {% if publi.link != null %} 
  <a href="{{ publi.link }}">[PDF]</a>
  {% endif %}

{% endfor %}
## Domestic Patents
{% assign var_year = 2030 %}
{% for publi in site.data.publications.domestic_patents %}
  {% if var_year != publi.year and var_year > year_until%}
  **{{ publi.year }}** <br />
  {% endif %}
  {% assign var_year = publi.year %}
  **{{ publi.title }}** <br />
  <em>{{ publi.authors }} </em><br />
  {{publi.info}}, {{ publi.year }}년 {{ publi.month }}월 {% if publi.link != null %}
  <a href="{{ publi.link }}">[PDF]</a>
  {% endif %}

{% endfor %}

## Invited Talks

{% for publi in site.data.publications.invited_talks %}

  **{{ publi.title }}** <br />
  {{publi.info}}, {{ publi.month }} {{ publi.year }}

{% endfor %}
