
[Back to Policies & Procedures](/)

### Rules of Procedure

{% assign pages = site.pages | where_exp: "page", "page.document contains 'Rules of Procedure'" | sort: 'title' | limit: 1000 %}
{% for p in pages %}

* {% if page.title == p.title %} {{p.title}} {% else %} {% unless p.url contains 'historical' %}[{{ p.title }}]({{ p.url }}){% endunless %}{% endif %}
{% endfor %}
