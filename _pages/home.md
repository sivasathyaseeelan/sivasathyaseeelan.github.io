---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">ML Interatomic Potentials</a>
<a href="{{ '/research' | relative_url }}" class="chip">Molecular Dynamics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Stochastic Simulation</a>
<a href="{{ '/research' | relative_url }}" class="chip">Materials Informatics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Cheminformatics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Electronic Structure</a>
<a href="{{ '/research' | relative_url }}" class="chip">GPU Computing</a>
</div>

I work at the intersection of computational chemistry and scientific machine learning: building machine-learned interatomic potentials, GPU-accelerated molecular and stochastic simulation software in Julia, and data-driven models that predict molecular and materials properties from chemical structure.

<div class="callout callout-success" markdown="0">
<div class="callout-title">{% include icon.html name="award" class="callout-icon" %} Google Summer of Code 2026 with JuliaMolSim</div>
<p>Implementing ANI-2x and E(3)-equivariant interatomic potentials natively in Julia for <a href="https://github.com/JuliaMolSim/Molly.jl">Molly.jl</a>, with analytic forces and portable GPU kernels that make Molly the fastest ANI implementation on a 15,954-atom protein. Mentored by Dr. Joe Greener (University of Cambridge).</p>
</div>

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

## About me

I am completing an Integrated Dual Degree (B.Tech + M.Tech) in Industrial Chemistry at the Indian Institute of Technology (BHU), Varanasi, where I work with [Dr. V. Ramanathan](https://scholar.google.com/citations?user=oLHHKoAAAAAJ) on machine learning for molecular property prediction, materials informatics, and flavour science, alongside *ab initio* studies of hydrogen bonding and chemometric analysis of Raman spectra.

In 2025 I was a SciML Fellow at the MIT Julia Lab, where I wrote GPU-accelerated Gillespie and tau-leaping solvers and variable-rate jump aggregators for JumpProcesses.jl, and a Summer of Reproducibility fellow at the UC Santa Cruz OSPO. In 2026 I am a Google Summer of Code contributor with JuliaMolSim, bringing native ANI-2x and equivariant potentials to Molly.jl. I also work as a Machine Learning Engineer at [Ema](https://www.ema.co), building LLM pipelines, localization systems, and observability for an agentic AI platform.

Outside research I captained the IIT (BHU) table tennis team and served as Deputy Contingent Leader for Inter-IIT Tech Meet 13.0, leading a contingent of 90+ members to two gold medals and a bronze.
