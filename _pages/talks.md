---
title: "Talks"
permalink: /talks/
author_profile: true
---

{% comment %} Each talk is a Markdown file in _talks/. See README.md. {% endcomment %}
{% assign talks = site.talks | sort: "date" | reverse %}
<ul class="talks">
{% for talk in talks %}{% include talk.html talk=talk %}{% endfor %}
</ul>

{% include verify.html note="add any other talks listed on the CV" %}
