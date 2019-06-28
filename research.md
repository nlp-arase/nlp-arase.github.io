---
layout: page
title : Research
permalink: /research/
category: "research"
tagline: "研究内容"
---

<div>
{% for UT in site.data.research %}
    <h3 class="member-role"><span>{{ UT.UpperTheme }}</span></h3>
    {% for LT in UT.LowerTheme %}
        <div class="member-content">
            <div class="research-theme">{{ LT.theme }}</div><BR>
            <div class="research-content">{{ LT.contents }}</div>
        </div>
    {% endfor %}
{% endfor %}
</div>