---

layout: col-generic
title: Policies & Procedures

---

<!-- rebuild 5 -->

## Rules of Procedure
Policies and Procedures adopted by the Global Board for OWASP Operations. Last edition: xxxx-xx-xx
{% assign pages = site.pages | where_exp: "page", "page.document contains 'Rules of Procedure'" | sort: 'title' | limit: 1000 %}
<ul>
{% for page in pages %}
 {% if page.path contains 'operational/' %}
 <li><a href="https://policy.owasp.org{{ page.url | replace: '.html', '' }}">{{ page.title }}</a></li>
 {% endif %}
{% endfor %}
</ul>

## Guidebooks

Handbooks to help Chapter, Project, and Event Leaders in their volunteer work.
{% assign pages = site.pages | sort: 'title' | limit: 1000 %}
<ul>
{% for page in pages %}
 {% if page.path contains 'guidebook/' %}
 <li><a href="https://policy.owasp.org{{ page.url | replace: '.html', '' }}">{{ page.title }}</a></li>
 {% endif %}
{% endfor %}
</ul>

## Contract and Agreement Templates

{% assign pages = site.pages | sort: 'title' | limit: 1000 %}
<ul>
{% for page in pages %}
 {% if page.path contains 'legal/' %}
 <li><a href="https://policy.owasp.org{{ page.url | replace: '.html', '' }}">{{ page.title }}</a></li>
 {% endif %}
{% endfor %}
</ul>
