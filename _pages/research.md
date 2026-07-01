---
layout: page
title: "Research"
permalink: /research/
description: "Research—Taesoo Song. Housing supply and neighborhood change, race and immigration, and data infrastructure."
rail_label: "On this page"
sections:
  - id: overview
    title: "Overview"
  - id: supply
    title: "Supply & neighborhoods"
  - id: race
    title: "Race & immigration"
  - id: data
    title: "Data infrastructure"
---

My research asks how housing supply—including both new construction and the ongoing transformation of the existing housing stock—shapes *who gets to live where*, and with what consequences for inequality. I pursue this across three connected pillars. See my [full list of publications](/publications/) or my [Google Scholar profile](https://scholar.google.com/citations?user=xM5Rc-EAAAAJ&hl=en).
{:.lead}
{:#overview}

## Housing supply and neighborhood change {#supply}

I examine how access to housing and neighborhoods is governed through housing supply and the everyday transformation of the existing housing stock. Methodologically, I leverage novel administrative and commercial data, combined with quantitative and geospatial approaches, to observe these processes at fine spatial and temporal scales and to connect policy, market, and housing-stock changes to household-level mobility outcomes.

### Neighborhood change, gentrification, and displacement

One strand examines how neighborhood change—gentrification, the loss of unsubsidized affordable housing, and rising prices—reshapes who can stay and who is pushed out, tracing these dynamics through household residential mobility.

{% assign items = site.data.publications.published | where: "subtheme", "neighborhoods" %}
{% include pub-list.html items=items %}

### Housing and land use policies

A second strand examines how explicit housing and land use policies—zoning reform, upzoning, and new construction—shape access and displacement risk. Debates about supply often focus narrowly on production, overlooking how the intensity, location, and form of development shape access differently across neighborhoods and groups; I ask when and where new supply mitigates or intensifies exclusion.

{% assign items = site.data.publications.published | where: "subtheme", "supply-policy" %}
{% include pub-list.html items=items %}

### Demolition and redevelopment

A third strand turns from new construction to the transformation of the existing stock—the demolitions, teardowns, and redevelopment that quietly reshape neighborhoods. I ask what demolition and redevelopment actually become on the ground—what replaces what is torn down, where, and for whom—using building permit and parcel records, and taking seriously the measurement choices involved in studying redevelopment with local administrative data.

{% assign items = site.data.publications.working | where: "subtheme", "demolition" %}
{% include pub-list.html items=items %}

<img class="figwide" src="/images/oaklandwalls.png" alt="Oakland streetscape">

## Race, immigration, and housing {#race}

This pillar uses **mixed methods** to examine how immigration reshapes—and is simultaneously shaped by—racialized boundaries of belonging in housing markets. Focusing on Asian populations in the United States and Canada, an underrepresented group in housing research, I trace how historical and contemporary land use regimes, housing policies, and racialized political and media narratives reproduce differential inclusion and inequality across scales.

### Divergent immigrant incorporation in housing access

My dissertation challenges the treatment of Asians as a monolithic "other" within the Black–White binary paradigm, arguing that this categorization reinforces racial inequality by perpetuating the "model minority" stereotype. I argue that prior research has obscured significant housing disparities within the diverse pan-ethnic Asian American community, and that by attending to this diversity, we can observe divergent patterns of incorporation. I also show how land use and housing policy continue to stratify Asian American housing outcomes despite significant gains in socioeconomic attainment, complicating contemporary narratives around race and class in housing access.

{% assign items = site.data.publications.working | where: "subtheme", "incorporation" %}
{% include pub-list.html items=items %}

<img class="figwide" src="/images/sfchinatown.png" alt="San Francisco Chinatown">

### Racialized narratives and legislating housing exclusion

While immigration debates have traditionally centered on labor market competition, housing affordability has emerged as a growing site of politicization—often with a focus on Asian, particularly Chinese, immigrants. Anglosphere countries such as Canada, Australia, and New Zealand have implemented taxes and restrictions aimed at limiting non-citizen home purchases, framing them as a response to rising housing costs. In the United States, Texas and Florida have legislated property-purchase bans targeting Chinese nationals, including immigrants in the country. I am interested in how such policies both reflect and reinforce racialized narratives of Asian immigrants, drawing on historical parallels such as the Alien Land Laws, and I quantitatively assess the impacts of these restrictive policies on the housing market.

{% assign items = site.data.publications.published | where: "subtheme", "narratives" %}
{% include pub-list.html items=items %}

<img class="figwide" src="/images/woman-anti-japanese-sign.jpg" alt="Historical anti-Japanese housing sign">

## Data infrastructure {#data}

Understanding housing and neighborhood exclusion requires measuring who moves, who stays, and who is missed entirely. My methodological work evaluates new consumer and administrative datasets for capturing residential mobility and exclusionary dynamics at fine spatial scales, while developing best practices to address the data biases that can distort the representation of marginalized and underrepresented groups.

I am extending this agenda to building permits and other local administrative data to study demolitions and property transformations—additions, alterations, and teardowns—and the planning and neighborhood conditions associated with them.

{% assign items = site.data.publications.published | where: "subtheme", "big-data" %}
{% include pub-list.html items=items %}
