---
layout: page
title : Research
permalink: /research/
tagline: "研究内容"
---

{% for UT in site.data.research %}
    <div class="member-role"><strong>{{ UT.UpperTheme }}</strong></div>
    {% for LT in UT.LowerTheme %}
    <div class="research-area">
        <div class="research-theme">{{ LT.theme }}</div><BR>
        <div class="research-content">{{ LT.contents }}</div>
    </div>
    {% endfor %}
{% endfor %}