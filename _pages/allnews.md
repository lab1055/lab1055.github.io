---
title: "Machine Learning and Vision Group - News"
layout: textlay
excerpt: "Machine Learning and Vision Group News"
sitemap: false
permalink: /allnews.html
---

<h1 class='page-header'>
News
</h1>

{% for article in site.data.news %}
<p><b>{{ article.date }}</b><br>
{{ article.headline }}</p>
{% endfor %}
