---

layout: col-generic
title: Policies & Procedures

---

<!-- rebuild 1 -->

## Rules of Procedure
Policies and Procedures adopted by the Global Board for OWASP Operations. Last edition: xxxx-xx-xx
{% assign pages = site.pages | where_exp: "page", "page.document contains 'Rules of Procedure'" | sort: 'title' | limit: 1000 %}
<ul>
{% for page in pages %}
 {% if page.path contains 'operational/' %}
 <li><a href='/www-policy{{ page.url }}'>{{ page.title }}</a></li>
 {% endif %}
{% endfor %}
</ul>

## Guidebooks
Handbooks to help Chapter, Project, and Event Leaders in their volunteer work.
{% assign pages = site.pages | sort: 'title' | limit: 1000 %}
<ul>
{% for page in pages %}
 {% if page.path contains 'guidebook/' %}
 <li><a href='/www-policy{{ page.url }}'>{{ page.title }}</a></li>
 {% endif %}
{% endfor %}
</ul>

## Contract and Agreement Templates
{% assign pages = site.pages | sort: 'title' | limit: 1000 %}
<ul>
{% for page in pages %}
 {% if page.path contains 'legal/' %}
 <li><a href='/www-policy{{ page.url }}'>{{ page.title }}</a></li>
 {% endif %}
{% endfor %}
</ul>

## Others
- [Employee Handbook](/www-policy/employee)

## TODO
- Contact Us (responsivness to tickets, SLA, submitting complete information, submitting accurate information)
- Membership - terms, discounts, submitting accurate info, pricing, honorary process, peference for Foundation events (like PRoject Summits etc
- Advertising
- Travel Assistance Program - member, workflow, limits, 
- Local Partnerships
- Mailing Lists
- Elections
- Licenses


