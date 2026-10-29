---
permalink: /
title: "Frank Yingjie Huo"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<p class="home-interests">{{ site.author.tagline }}</p>

<p class="home-links">
{% if site.author.email %}<a href="mailto:{{ site.author.email }}">Email</a>{% else %}Email {% include verify.html %}{% endif %}
· <a href="{{ site.author.googlescholar }}">Google Scholar</a>
· {% include cv-link.html label="CV" %}
</p>

I am a PhD candidate in Theoretical Physics at George Washington University, and expect to complete my PhD in May 2027. I am fortunate to be advised by Prof. Neil F. Johnson. Before my PhD, I studied at Pembroke College, University of Cambridge, where I received a BA in Physics (Natural Sciences Tripos) and an MMath (Part III of the Mathematical Tripos).
{: .home-intro}

I develop exactly solvable models of collective dynamics in complex systems. I currently focus on the dynamics of Transformer-based AI, from the microscopic scale of a single attention head to the coarse-grained level of a whole conversation. In recent work, together with Prof. Johnson, we show from first principles that the attention mechanism sets up a competition between tokens during text generation, analogous to two-body interactions in a multispin system, which leads to token repetition and tipping between outputs ([*AIP Advances*, 2026](https://doi.org/10.1063/5.0296911)); trace how this competition propagates through the layers of a Transformer ([arXiv, 2026](https://arxiv.org/abs/2607.25279)); and test a simple criterion for good-to-bad tipping against observations of real models ([*Patterns*, 2026](https://doi.org/10.1016/j.patter.2026.101666)).

Earlier in my PhD, I developed theories of heterogeneous assembly and fragmentation dynamics on complex networks, and applied them to real-world systems, online and offline ([PRL 2023](https://doi.org/10.1103/PhysRevLett.130.237401), [2024](https://doi.org/10.1103/PhysRevLett.133.247401)). These theories are set out in full, with substantial new results, in our book [*Introduction to Online Complexity*](https://global.oup.com/academic/product/introduction-to-online-complexity-9780198921011) (Oxford University Press, 2025), of which I am lead author. A full list of my work is on the [Publications]({{ "/publications/" | relative_url }}) page. {% include verify.html note="draft research paragraphs: check wording" %}

For five years {% include verify.html note="years" %} I have been a teaching assistant in the Department of Physics at George Washington University, in Nonlinear Dynamics and General Physics. I run office hours as Cambridge-style small-group supervisions, where students work through problems themselves and I diagnose where their understanding breaks down. I received the Bennhold Family Award for best graduate-student teaching {% include verify.html note="year" %}. [More on teaching →]({{ "/teaching/" | relative_url }})
