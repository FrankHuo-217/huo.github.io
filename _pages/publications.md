---
title: "Publications"
permalink: /publications/
author_profile: true
---

{% comment %} Each publication is a Markdown file in _publications/. See README.md. {% endcomment %}
A complete list is on [Google Scholar]({{ site.author.googlescholar }}).
{: .page-lede}

{% for category in site.publication_category %}
  {% assign pubs = site.publications | where: "category", category[0] | where_exp: "p", "p.hide != true" | sort: "date" | reverse %}
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

## In the media

Our recent [*Patterns* paper](https://doi.org/10.1016/j.patter.2026.101666) on good-to-bad tipping in AI has received international coverage, including in [*The Independent*](https://www.the-independent.com/tech/rogue-ai-artificial-intelligence-maths-b3063619.html), [*El País*](https://elpais.com/tecnologia/2026-10-08/la-ia-no-distingue-el-bien-del-mal-dos-fisicos-destapan-lo-que-las-grandes-empresas-quieren-esconder.html), [*Nautilus*](https://nautil.us/a-recipe-for-stopping-ai-from-going-rogue-1285647), [*Live Science*](https://www.livescience.com/technology/artificial-intelligence/simple-math-can-predict-when-ai-is-about-to-go-rogue-physicists-say), [*SecurityWeek*](https://www.securityweek.com/formula-predicts-when-ai-chatbots-are-at-risk-of-turning-bad/) and [*Decrypt*](https://decrypt.co/380624), and an [InvestigateTV](https://www.wbtv.com/2026/10/20/what-happens-when-good-ai-goes-bad-researchers-studying-tipping-point/) report carried by local television stations across the United States.
