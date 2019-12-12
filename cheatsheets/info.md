{% assign cheatsheets = site.pages | where_exp: "page", "page.tags contains page.document" %}
<ul>
{% for page in cheatsheets %}
<li><a href="{{site.github.url}}{{page.url}}">{{ page.title }}</a></li>
<hr style="border: 1px solid darkgray; margin-left: 27%; max-width: 33%;">
{% endfor %}
</ul>