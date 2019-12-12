{% assign cheatsheets = site.pages | where_exp: "page", "page.tags contains page.document" %}
<ul>
{% for page in cheatsheets %}
<li><a href="{{site.github.url}}{{page.url}}">{{ page.title }}</a></li>
{% endfor %}
</ul>