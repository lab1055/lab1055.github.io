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
<p style="color: #76838f"><span style="font-family: monaco, monospace; background-color: #c2f5ff94; color: #526069">({{ article.date }})</span>: {{ article.headline }}</p>
{% endfor %}
