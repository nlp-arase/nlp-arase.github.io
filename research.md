---
layout: page
title : Research
permalink: /research/
---

<h2>研究内容</h2>
{% for UT in site.data.research %}
    <div class="manual-post">
        <div class="manual manual-title">
            <strong>{{ UT.UpperTheme }}</strong>
        </div>
    {% for LT in UT.LowerTheme %}
        <span class="manual">{{ LT.theme }}</span><BR>
        <div class="manual-content">
            <pre>{{ LT.contents }}</pre>
        </div>
    {% endfor %}
    </div>
{% endfor %}
