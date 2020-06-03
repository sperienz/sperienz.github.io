---
layout: default
title: Event List
---

<!-- Html Elements for Search -->
<section class="posts">
<h3>External Links</h3>
<ul>
{% for link in site.events %}
<li><a href="{{ site.baseurl }}{{ link.url }}">{{ link.title }}</a><time datetime="{{ link.date | date_to_xmlschema }}">{{ link.date | date: "%m-%d-%Y" }}</time></li>
{% endfor %}
</ul>
</section>

