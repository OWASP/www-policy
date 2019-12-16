---

layout: col-generic
title: Policies & Procedures

---

## Rules of Procedure
Policies and Procedures adopted by the Global Board for OWASP Operations. Last edition: xxxx-xx-xx
{% assign pages = site.pages | sort: 'title' | limit: 1000 %}
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

## Legal
Contract and Agreement Templates
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
- Donations - unrestricted, restricted and process. Being listed as a supporter
- Contact Us (responsivness to tickets, SLA, submitting complete information, submitting accurate information)
- Membership - terms, discounts, submitting accurate info, pricing, honorary process, peference for Foundation events (like PRoject Summits etc
- Acknowledgements
- Advertising
- Local Event Policies
- Travel Assistance Program - member, workflow, limits, 
- Grants
- Local Partnerships
- Mailing Lists
- Elections
- Licenses


