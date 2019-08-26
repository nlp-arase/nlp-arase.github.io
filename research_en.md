---
layout: page
title : Research
permalink: /research/
category: "research"
tagline: "研究内容"
lang: en
---

<div>
{% for UT in site.data.research %}
    <h3 class="member-role"><span>{{ UT.UpperTheme_en }}</span></h3>
    {% for LT in UT.LowerTheme %}
        <div class="research-area">
            <div class="research-theme">{{ LT.theme_en }}</div><BR>
            <div class="research-content">{{ LT.contents_en }}</div>
        </div>
    {% endfor %}
{% endfor %}
</div>