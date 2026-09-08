---
title: "Research"
layout: page
permalink: /research/
---

# Research

My research combines computational chemistry with scientific machine learning. I build fast, open-source simulation software in Julia (machine-learned interatomic potentials, GPU kernels, stochastic solvers) and data-driven models that connect chemical structure to molecular and materials properties.

<div class="research-grid">

<div class="research-card">
<img src="{{ '/images/research/mlip.svg' | relative_url }}" class="research-thumb" width="400" height="200" alt="Atomic environment feeding a neural network potential">
<div class="research-body">
<h2 class="research-title">Machine-Learned Interatomic Potentials</h2>
<p class="research-desc">Native Julia implementations of ANI-2x and E(3)-equivariant (NequIP, Allegro) potentials for <a href="https://github.com/JuliaMolSim/Molly.jl">Molly.jl</a>, with analytic forces from custom backpropagation through atomic environment vectors and portable GPU kernels (CUDA, Metal, ROCm). Benchmarked against TorchANI and NNPOps, the CUDA path is the fastest on a 15,954-atom protein. Google Summer of Code 2026 with JuliaMolSim.</p>
</div>
</div>

<div class="research-card">
<img src="{{ '/images/research/stochastic.svg' | relative_url }}" class="research-thumb" width="400" height="200" alt="Stochastic jump trajectories">
<div class="research-body">
<h2 class="research-title">Stochastic Simulation and SciML</h2>
<p class="research-desc">Exact Gillespie SSA and tau-leaping solvers with hand-tuned GPU kernels, variable-rate jump aggregators for state- and time-dependent rates coupled to ODEs, and GPU Poisson sampling for <a href="https://github.com/SciML/JumpProcesses.jl">JumpProcesses.jl</a> and PoissonRandom.jl, validated on epidemiological and chemical-reaction-network models. SciML Fellowship 2025 at the MIT Julia Lab.</p>
</div>
</div>

<div class="research-card">
<img src="{{ '/images/research/materials.svg' | relative_url }}" class="research-thumb" width="400" height="200" alt="Grid of elements and a band-gap curve">
<div class="research-body">
<h2 class="research-title">Materials Informatics</h2>
<p class="research-desc">Predicting semiconductor band gaps directly from elemental composition, benchmarking Random Forest, XGBoost, artificial neural networks, and graph neural networks for high-throughput materials screening. Published in <em>Scientific Reports</em> (2026).</p>
</div>
</div>

<div class="research-card">
<img src="{{ '/images/research/cheminformatics.svg' | relative_url }}" class="research-thumb" width="400" height="200" alt="Molecular graph mapped to fingerprint bits">
<div class="research-body">
<h2 class="research-title">Cheminformatics and Flavour Science</h2>
<p class="research-desc">Multi-label and multi-class classifiers that predict a molecule's taste profile (sweet, bitter, sour, and more) from its structure using molecular fingerprints and descriptors, plus a study of how stereochemical ambiguity in SMILES (chiral centres, E/Z isomerism) degrades molecular property prediction.</p>
</div>
</div>

<div class="research-card">
<img src="{{ '/images/research/electronic.svg' | relative_url }}" class="research-thumb" width="400" height="200" alt="Sulfur-centred hydrogen bond">
<div class="research-body">
<h2 class="research-title">Electronic Structure of Hydrogen Bonds</h2>
<p class="research-desc"><em>Ab initio</em> studies of sulfur-centred hydrogen-bond cooperativity in ethane-1,2-dithiol clusters interacting with HF, H<sub>2</sub>O, and NH<sub>3</sub>, quantifying how cluster size strengthens these weak interactions. Published in <em>Physical Chemistry Chemical Physics</em> (2026).</p>
</div>
</div>

<div class="research-card">
<img src="{{ '/images/research/chemometrics.svg' | relative_url }}" class="research-thumb" width="400" height="200" alt="Raman spectra and PCA scores">
<div class="research-body">
<h2 class="research-title">Chemometrics and Spectroscopy</h2>
<p class="research-desc">A consensus chemometric pipeline (PCA, PLS-DA, K-Means, VIP, SIMCA) over full-spectrum Raman data across three wavenumber ranges that authenticates commercial ghee against reference fats, flagging lard adulteration and ruling out palm oil.</p>
</div>
</div>

</div>
