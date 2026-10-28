---
permalink: /
title: "Frank Yingjie Huo"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<p class="home-affil">
PhD candidate in Theoretical Physics, George Washington University<br>
Advisor: Neil F. Johnson
</p>

<p class="home-interests">Exactly solvable many-body dynamics, from complex networks to Transformer AI</p>

<p class="home-links">
<a href="mailto:{{ yfh400@gwu.edu }}">Email</a>
· <a href="{{ site.author.googlescholar }}">Google Scholar</a>
· {% include cv-link.html label="CV" %}
</p>

## Research

I develop exactly solvable models of collective dynamics in complex systems, currently focused on the dynamics of Transformer-based AI. By mapping the attention mechanism onto a multispin system, I derive closed-form conditions for when a model's output tips between competing basins of behavior, governed by dot-product competition between the context and those basins. I use a vector generalization of fusion–fission dynamics to track how these basins form as tokens propagate through the network. Earlier work developed multi-species fusion–fission theory for the assembly and breakup of groups online and offline ([PRL 2023]({{ "/publications/#2023-prl-shockwavelike-behavior" | relative_url }}), [2024]({{ "/publications/#2024-prl-multispecies-cohesion" | relative_url }})). This theory, with substantial new results, is developed in my [Oxford University Press book]({{ "/publications/#2025-book-introduction-to-online-complexity" | relative_url }}). {% include verify.html note="draft paragraph: check wording" %}

## Selected publications

{% assign selected = site.publications | where_exp: "p", "p.selected" | sort: "selected" %}
{% include publication-list.html pubs=selected %}

[All publications →]({{ "/publications/" | relative_url }})

## Teaching

Teaching assistant in the Department of Physics at George Washington University for five years {% include verify.html note="years" %}, in **Nonlinear Dynamics** (instructor: Prof. Neil Johnson) and **General Physics**. I run office hours as Cambridge-style small-group supervisions: students work through problems themselves, and I diagnose where their understanding breaks down. Recipient of the **Bennhold Family Award** for best graduate-student teaching {% include verify.html note="year" %}.

[More on teaching →]({{ "/teaching/" | relative_url }})

## Education

- **PhD in Physics** {% include verify.html note="official degree name" %}, George Washington University, expected {% include verify.html note="date" %}. Advisor: Neil F. Johnson.
- **BA, MA and MMath (Part III of the Mathematical Tripos)**, Pembroke College, University of Cambridge.
