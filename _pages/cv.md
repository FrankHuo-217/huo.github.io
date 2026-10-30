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

- **PhD in Physics**, George Washington University, expected May 2027. Columbian Distinguished Fellow. Advisor: Neil F. Johnson.
- **MMath** (Part III of the Mathematical Tripos) and **BA in Physics** (Natural Sciences Tripos), Pembroke College, University of Cambridge, 2021; MA (Cantab), 2025. Foundation Scholar; Foundress Prize.

## Awards and honors

- **SIAM Student Travel Award**, SIAM Annual Meeting (AN26), 2026
- **Scholar**, [Edward A. Bouchet Graduate Honor Society](https://columbian.gwu.edu/edward-alexander-bouchet-graduate-honor-society), 2026
- **Gus W. Weiss Prize** for Outstanding Student in Physics, George Washington University, 2026
- **Parke Prize** for Excellence in Theoretical Physics, George Washington University, 2024
- **Bennhold Family Award** for best graduate-student teaching, George Washington University, 2022

## Talks

{% comment %} Each talk is a Markdown file in _talks/. See README.md. {% endcomment %}
{% assign talks = site.talks | sort: "date" | reverse %}
<ul class="talks">
{% for talk in talks %}{% include talk.html talk=talk %}{% endfor %}
</ul>

## Refereeing

Referee for *Physical Review Letters*, *Physical Review E*, and *Patterns*.

## Research and teaching

- [Publications]({{ "/publications/" | relative_url }}): one book (Oxford University Press), journal articles including two in *Physical Review Letters*, and preprints.
- [Teaching]({{ "/teaching/" | relative_url }}): teaching assistant in physics since 2021, in four courses from introductory physics to nonlinear dynamics.
