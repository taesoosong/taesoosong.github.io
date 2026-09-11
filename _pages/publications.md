---
layout: page
title: "Publications"
permalink: /publications/
description: "Publications — Taesoo Song. Journal articles, policy research, reviews, and public scholarship on housing and cities."
rail_label: "Scholarship"
sections:
  - id: "articles"
    title: "Journal articles"
  - id: "policy"
    title: "Policy briefs"
  - id: "reviews"
    title: "Book reviews"
  - id: "public"
    title: "Public scholarship"
  - id: "working"
    title: "Work in progress"
---

<p class="lead">Research on housing supply, neighborhood change, immigration, and the data used to understand cities.</p>

{% assign articles = site.data.publications.articles %}
{% assign total = articles | size %}
<h2 id="articles">Peer-reviewed journal articles</h2>
{% for p in articles %}
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

<h2 id="policy">Policy briefs</h2>
{% include pub-list.html items=site.data.publications.policy %}

<h2 id="reviews">Book reviews</h2>
{% include pub-list.html items=site.data.publications.reviews %}

<h2 id="public">Public scholarship</h2>
{% include pub-list.html items=site.data.publications.public_scholarship %}

<h2 id="working">Work in progress</h2>
{% include pub-list.html items=site.data.publications.working %}
