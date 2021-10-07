---
title: "News"
layout: textlay
excerpt: "InRobots Lab at Jilin University."
sitemap: false
permalink: /InRobotsnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
