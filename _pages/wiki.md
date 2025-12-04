---
layout: page
title: COST FinAI Wiki Archive
permalink: /wiki/
---

# EU COST FinAI Wiki Archive

This section contains archived content from **wiki.fin-ai.eu**, the wiki for the COST Action CA19130 "Fintech and Artificial Intelligence in Finance" and the MSCA Digital Finance Industrial Doctoral Network.

The original wiki is no longer available, so this content has been preserved via the [Wayback Machine](https://web.archive.org/).

## Categories

{% for cat in site.data.wiki.categories %}
### {{ cat.name | capitalize }}
{{ cat.count }} pages

{% assign cat_pages = site.wiki | where: "category", cat.name %}
{% for page in cat_pages %}
- [{{ page.title }}]({{ page.url | relative_url }})
{% endfor %}

{% endfor %}

---

*Content archived from wiki.fin-ai.eu via the Internet Archive Wayback Machine.*
