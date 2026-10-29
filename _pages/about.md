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

I develop exactly solvable models of collective dynamics in complex systems, currently focused on the dynamics of Transformer-based AI. By mapping the attention mechanism onto a multispin system, I derive closed-form conditions for when a model's output tips between competing basins of behavior, governed by dot-product competition between the context and those basins. I use a vector generalization of fusion–fission dynamics to track how these basins form as tokens propagate through the network. Earlier work developed multi-species fusion–fission theory for the assembly and breakup of groups online and offline ([PRL 2023]({{ "/publications/#2023-prl-shockwavelike-behavior" | relative_url }}), [2024]({{ "/publications/#2024-prl-multispecies-cohesion" | relative_url }})). This theory, with substantial new results, is developed in my [Oxford University Press book]({{ "/publications/#2025-book-introduction-to-online-complexity" | relative_url }}). {% include verify.html note="draft paragraph: check wording" %}

Selected publications include my book [*Introduction to Online Complexity: The New Social Physics of Extremes, Misinformation, and AI*]({{ "/publications/#2025-book-introduction-to-online-complexity" | relative_url }}) (Oxford University Press, 2025), of which I am lead author and which contains substantial original research beyond my published papers, and, on Transformer dynamics, [*Competition for attention predicts good-to-bad tipping in AI*]({{ "/publications/#2026-patterns-competition-for-attention" | relative_url }}) (*Patterns*, 2026; equal contribution with Neil F. Johnson), [*Simple picture of how output from ChatGPT-like AI shifts from good to bad*]({{ "/publications/#2026-pnas-nexus-good-to-bad" | relative_url }}) (*PNAS Nexus*, 2026) and [*Physics of generative AI's atom: Repetition, bias, and beyond*]({{ "/publications/#2026-aip-advances-generative-ai-atom" | relative_url }}) (*AIP Advances*, 2026). [All publications →]({{ "/publications/" | relative_url }})

For five years {% include verify.html note="years" %} I have been a teaching assistant in the Department of Physics at George Washington University, in Nonlinear Dynamics and General Physics. I run office hours as Cambridge-style small-group supervisions, where students work through problems themselves and I diagnose where their understanding breaks down. I received the Bennhold Family Award for best graduate-student teaching {% include verify.html note="year" %}. [More on teaching →]({{ "/teaching/" | relative_url }})
