---
title: "Publications"
permalink: /publications/
author_profile: true
---

{% comment %} Each publication is a Markdown file in _publications/. See README.md. {% endcomment %}
Also on [Google Scholar]({{ site.author.googlescholar }}).
{: .page-lede}

{% for category in site.publication_category %}
  {% assign pubs = site.publications | where: "category", category[0] | sort: "date" | reverse %}
  {% if pubs.size == 0 %}{% continue %}{% endif %}
  {% if category[1].collapsed %}
<details class="pubs-collapsed">
<summary><h2 id="{{ category[0] }}">{{ category[1].title }} ({{ pubs.size }})</h2></summary>
{% include publication-list.html pubs=pubs %}
</details>
  {% else %}
<h2 id="{{ category[0] }}">{{ category[1].title }}</h2>
{% include publication-list.html pubs=pubs %}
  {% endif %}
{% endfor %}

## Code

{% include verify.html note="add links to public code repositories, or delete this section" %}

## In the media

Coverage of *Competition for attention predicts good-to-bad tipping in AI* (*Patterns*, 2026): [Live Science](https://www.livescience.com/technology/artificial-intelligence/simple-math-can-predict-when-ai-is-about-to-go-rogue-physicists-say), [Nautilus](https://nautil.us/a-recipe-for-stopping-ai-from-going-rogue-1285647), [InvestigateTV](https://www.wbtv.com/2026/10/20/what-happens-when-good-ai-goes-bad-researchers-studying-tipping-point/), The Independent {% include verify.html note="link" %}, El País {% include verify.html note="link" %}.
