---
layout: page
title : Research
permalink: /research/
category: "research"
tagline: "研究内容"
---

{% for UT in site.data.research %}
    <span>{{ UT.UpperTheme }}</span>
    {% for LT in UT.LowerTheme %}
        <div class="research-theme">{{ LT.theme }}</div><BR>
        <div class="research-content">{{ LT.contents }}</div>
    {% endfor %}
{% endfor %}