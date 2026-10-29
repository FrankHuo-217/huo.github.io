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

I am a PhD candidate in Theoretical Physics at George Washington University, advised by Neil F. Johnson, and expect to complete my PhD in {% include verify.html note="month and year" %}. Before that, I studied at Pembroke College, University of Cambridge, where I received a BA in Physics (Natural Sciences Tripos) and an MMath (Part III of the Mathematical Tripos).
{: .home-intro}

I develop exactly solvable models of collective dynamics in complex systems. I currently focus on the dynamics of Transformer-based AI, from the microscopic scale of a single attention head to the coarse-grained level of a whole conversation. In recent work, we show from first principles that the attention mechanism sets up a competition between tokens during text generation, analogous to two-body interactions in a multispin system, which leads to token repetition and tipping between outputs ([*AIP Advances*, 2026]({{ "/publications/#2026-aip-advances-generative-ai-atom" | relative_url }})); trace how this competition propagates through the layers of a Transformer ([arXiv, 2026]({{ "/publications/#2026-arxiv-many-body-tipping" | relative_url }})); and, combining the theory with observations of real models, predict when a model's output tips from good to bad ([*Patterns*, 2026]({{ "/publications/#2026-patterns-competition-for-attention" | relative_url }})).

Earlier work developed multi-species fusion–fission theory for the assembly and breakup of groups online and offline ([PRL 2023]({{ "/publications/#2023-prl-shockwavelike-behavior" | relative_url }}), [2024]({{ "/publications/#2024-prl-multispecies-cohesion" | relative_url }})). This theory, with substantial new results, is developed in my [Oxford University Press book]({{ "/publications/#2025-book-introduction-to-online-complexity" | relative_url }}). We have since extended it to AI: a vector generalization of fusion–fission dynamics forecasts, at the level of a whole conversation, when a model's behavior will shift from desirable to undesirable ([arXiv, 2026]({{ "/publications/#2026-arxiv-fusion-fission-forecasts" | relative_url }})). A full list of my work is on the [Publications]({{ "/publications/" | relative_url }}) page. {% include verify.html note="draft research paragraphs: check wording" %}

For five years {% include verify.html note="years" %} I have been a teaching assistant in the Department of Physics at George Washington University, in Nonlinear Dynamics and General Physics. I run office hours as Cambridge-style small-group supervisions, where students work through problems themselves and I diagnose where their understanding breaks down. I received the Bennhold Family Award for best graduate-student teaching {% include verify.html note="year" %}. [More on teaching →]({{ "/teaching/" | relative_url }})
