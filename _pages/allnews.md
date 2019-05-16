---
title: "Machine Learning and Vision Group - News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /allnews.html
---

<h1 class='page-header'>
News
</h1>

{% for article in site.data.news %}
<p><b>{{ article.date }}</b><br>
<em>{{ article.headline }}</em></p>
{% endfor %}
