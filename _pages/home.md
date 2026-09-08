---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero"><span class="name-first">{{ site.name_first | default: site.name }}</span>{% if site.name_first %} <span class="name-last">{{ site.name_last }}</span>{% endif %}</h1>
<p class="home-hero-sub">{{ site.title | replace: " · ", '<span class="sep">&middot;</span>' }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">ML Interatomic Potentials</a>
<a href="{{ '/research' | relative_url }}" class="chip">Molecular Dynamics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Stochastic Simulation</a>
<a href="{{ '/research' | relative_url }}" class="chip">Materials Informatics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Cheminformatics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Electronic Structure</a>
<a href="{{ '/research' | relative_url }}" class="chip">GPU Computing</a>
</div>

## About me

I am completing an Integrated Dual Degree (B.Tech + M.Tech) in Industrial Chemistry at the Indian Institute of Technology (BHU), Varanasi, where I work with [Dr. V. Ramanathan](https://scholar.google.com/citations?user=oLHHKoAAAAAJ) on machine learning for molecular property prediction, materials informatics, and flavour science, alongside *ab initio* studies of hydrogen bonding and chemometric analysis of Raman spectra.

In 2025 I was a SciML Fellow at the MIT CSAIL Julia Lab, advised by [Dr. Samuel A. Isaacson](https://scholar.google.com/citations?user=Ap9PfVQAAAAJ) and [Dr. Christopher Rackauckas](https://scholar.google.com/citations?user=1kyW6dwAAAAJ), where I wrote GPU-accelerated Gillespie and tau-leaping solvers and variable-rate jump aggregators for JumpProcesses.jl. The same summer I was a Summer of Reproducibility fellow at the UC Santa Cruz OSPO with [Dr. Ben Greenman](https://scholar.google.com/citations?user=3A9hNTEAAAAJ), building an LLM-based agent and a benchmark for type narrowing in gradual type checkers. In 2026 I am a Google Summer of Code contributor with JuliaMolSim, mentored by [Dr. Joe G. Greener](https://scholar.google.com/citations?user=IG6H3tIAAAAJ) at the University of Cambridge, bringing native ANI-2x and equivariant potentials to Molly.jl. I also work as a Machine Learning Engineer at [Ema](https://www.ema.co), building LLM pipelines, localization systems, and observability for an agentic AI platform.

Outside research I captained the IIT (BHU) table tennis team and served as Deputy Contingent Leader for Inter-IIT Tech Meet 13.0, leading a contingent of 90+ members to two gold medals and a bronze.

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}
