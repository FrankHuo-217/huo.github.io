---
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
  - /talks/
---

<p class="cv-download"><i class="fas fa-file-pdf" aria-hidden="true"></i> {% include cv-link.html label="Download CV (PDF)" %}</p>

## Education

- **PhD in Physics** {% include verify.html note="official degree name" %}, George Washington University, expected May 2027. Advisor: Neil F. Johnson.
- **MMath (Part III of the Mathematical Tripos)**, Pembroke College, University of Cambridge, {% include verify.html note="year" %}
- **BA in Physics (Natural Sciences Tripos)**, Pembroke College, University of Cambridge, {% include verify.html note="year" %}; MA (Cantab) {% include verify.html note="year" %}

## Awards and fellowships

- **Columbian Distinguished Fellowship**, Columbian College of Arts and Sciences, George Washington University, {% include verify.html note="years, e.g. 2021–2027" %}
- **Bennhold Family Award** for best graduate-student teaching, 2022
- **Bouchet Graduate Honor Society** {% include verify.html note="exact name and year of induction" %}
- **Weiss Prize** {% include verify.html note="awarding body and year" %}
- **Parke Prize** {% include verify.html note="awarding body and year" %}

## Talks

{% comment %} Each talk is a Markdown file in _talks/. See README.md. {% endcomment %}
{% assign talks = site.talks | sort: "date" | reverse %}
<ul class="talks">
{% for talk in talks %}{% include talk.html talk=talk %}{% endfor %}
</ul>

{% include verify.html note="add any other talks listed on the CV" %}

## Refereeing

Referee for *Physical Review Letters*, *Physical Review E* and *Patterns*.

## Research and teaching

- [Publications]({{ "/publications/" | relative_url }}): one book (Oxford University Press), journal articles including two in *Physical Review Letters*, and preprints.
- [Teaching]({{ "/teaching/" | relative_url }}): five years as a teaching assistant in physics, including Nonlinear Dynamics.
