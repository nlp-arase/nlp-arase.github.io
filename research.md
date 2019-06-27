---
layout: page
title : Research
permalink: /research/
---

<h2>研究内容</h2>

{% for UT in site.data.research %}
    <div class="member-role"><strong>{{ UT.UpperTheme }}</strong></div>
    {% for LT in UT.LowerTheme %}
    <div class="research-area">
        <span class="research-theme">{{ LT.theme }}</span><BR>
        <div class="research-content">{{ LT.contents }}</div>
    </div>
    {% endfor %}
{% endfor %}