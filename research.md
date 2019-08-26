---
layout: page
title : Research
permalink: /research/
category: "research"
tagline: "研究内容"
lang: ja
---

<div>
{% for UT in site.data.research %}
    <h3 class="member-role"><span>{{ UT.UpperTheme }}</span></h3>
    {% for LT in UT.LowerTheme %}
        <div class="research-area">
            <div class="research-theme">{{ LT.theme }}</div><BR>
            <div class="research-content">{{ LT.contents }}</div>
            {% for image in LT.img %}
                <div class="research-img" style="background: url({{ site.baseurl }}/image/{{ image }})"></div>
            {% endfor %}
        </div>
    {% endfor %}
{% endfor %}
</div>