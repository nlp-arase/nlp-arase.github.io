---
layout: page
title: Publication
permalink: /publication/
category: "science"
tagline: "荒瀬班の研究業績"
---


<h3 class="publication-genre"><span>受賞</span></h3> 

<ol>
{% for entry in site.data.awards %}
    <li class="publication-content" id="award">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>

<h3 class="publication-genre"><span>学術論文</span></h3> 

<ol>
{% for entry in site.data.journalPapers %}
    <li class="publication-content" id="journal">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>

<h3 class="member-role"><span>国際会議</span></h3> 

<ol>
{% for entry in site.data.internationalConferenceProceedings %}
    <li class="publication-content" id="journal">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>

<h3 class="member-role"><span>国内会議・研究会</span></h3> 

<ol>
{% for entry in site.data.domesticConferenceProceedings %}
    <li class="publication-content" id="journal">
        <div class="title">{{ entry.title }}</div>
        <div class="authors">{{ entry.authors }}</div>
        <div class="info">{{ entry.info }}</div>
    </li>
{% endfor %}
</ol>