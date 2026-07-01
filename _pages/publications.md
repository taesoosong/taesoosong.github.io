---
layout: page
title: "Publications"
permalink: /publications/
description: "Publications — Taesoo Song. Housing supply, residential mobility, segregation, and immigration."
rail_label: "Jump to"
sections:
  - id: "y2026"
    title: "2026"
  - id: "y2025"
    title: "2025"
  - id: "y2024"
    title: "2024"
  - id: "working"
    title: "Under review & in prep"
---

For the complete record, see my [Google Scholar profile](https://scholar.google.com/citations?user=xM5Rc-EAAAAJ&hl=en).
{:.lead}

{% assign pubs = site.data.publications.published %}
{% assign total = pubs | size %}
{% assign curyear = "" %}
{% for p in pubs %}
{% if p.year != curyear %}{% assign curyear = p.year %}
<h2 id="y{{ p.year }}">{{ p.year }}</h2>
{% endif %}
{% assign num = total | minus: forloop.index0 %}
{% capture cite %}{{ p.authors }} ({{ p.year }}). {% if p.url %}[{{ p.title }}.]({{ p.url }}){% else %}{{ p.title }}.{% endif %} {{ p.venue }}.{% endcapture %}
<div class="pub">
<span class="pub-num">{{ num }}.</span>
<div class="pub-body">
<p class="pub-cite">{{ cite | markdownify | remove: '<p>' | remove: '</p>' | strip }}</p>
{% if p.links %}<p class="pub-links">{% for l in p.links %}<a href="{{ l.url }}">{{ l.text }}</a>{% unless forloop.last %} &middot; {% endunless %}{% endfor %}</p>{% endif %}
</div>
</div>
{% endfor %}

<h2 id="working">Under review &amp; in preparation</h2>
{% for p in site.data.publications.working %}
{% capture cite %}{{ p.authors }} {{ p.title }}.{% endcapture %}
<div class="pub">
<span class="pub-num"></span>
<div class="pub-body">
<p class="pub-cite">{{ cite | markdownify | remove: '<p>' | remove: '</p>' | strip }} <span class="pub-status">{{ p.status }}</span></p>
</div>
</div>
{% endfor %}
