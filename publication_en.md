---
layout: page
title: Publication
permalink: /en/publication/
category: "science"
tagline: "荒瀬班の研究業績"
lang: en
---


<h3 class="publication-genre"><span>Awards</span></h3> 

<ol>
{% for entry in site.data.awards %}
    <li class="publication-content" id="award">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>

<h3 class="publication-genre"><span>Journal</span></h3> 

<ol>
{% for entry in site.data.journalPapers %}
    <li class="publication-content" id="journal">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>

<h3 class="member-role"><span>Conference</span></h3> 

<ol>
{% for entry in site.data.internationalConferenceProceedings %}
    <li class="publication-content" id="journal">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>