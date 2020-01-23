
[Back to Policies & Procedures](/www-policy/)

### Rules of Procedure
{% assign pages = site.pages | where_exp: "page", "page.path contains 'operational/'" | sort: 'title' | limit: 1000 %}
{% for p in pages %}
* {% if page.title == p.title %} {{p.title}} {% else %} [{{ p.title }}]({{ p.url }}){% endif %}
{% endfor %}
