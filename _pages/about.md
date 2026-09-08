---
title: "About"
layout: page
permalink: /about/
---

# About

<div class="section-card">
<div class="pi-card">
<img src="{{ site.photo | prepend: '/images/' | relative_url }}" class="pi-photo" alt="{{ site.name }}" width="160" height="160">
<div>
<h2 class="pi-name">{{ site.name }}</h2>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email" aria-label="Email">{% include icon.html name="envelope" %}</a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.links.cv | prepend: '/' | relative_url }}" class="icon-link" title="CV" aria-label="CV">{% include icon.html name="cv" %}</a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar" aria-label="Google Scholar">{% include icon.html name="google-scholar" %}</a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub" aria-label="GitHub">{% include icon.html name="github" %}</a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn" aria-label="LinkedIn">{% include icon.html name="linkedin" %}</a>{% endif %}
</div>
<p style="margin-top: var(--space-4);">Chennai, Tamil Nadu, India</p>
</div>
</div>
</div>

<div class="section-card">
<h3>Education</h3>
<ul>
<li><strong>Integrated Dual Degree (B.Tech + M.Tech), Industrial Chemistry</strong>, Indian Institute of Technology (BHU), Varanasi. Nov. 2021 &ndash; 2026. CPI 8.43 / 10.</li>
<li><strong>Master's thesis:</strong> <em>Applications of Machine Learning and Deep Learning in Predictive Analytics for Molecular Property Prediction, Materials Informatics, and Flavor Science</em>. Advisor: <a href="https://scholar.google.com/citations?user=oLHHKoAAAAAJ">Dr. V. Ramanathan</a>. <a href="https://drive.google.com/file/d/1E3fVMT5ZIxL68imjDSoBYnDfVAlDY97j/view" target="_blank">PDF</a></li>
</ul>
</div>

{% if site.data.awards %}
<div class="section-card">
<h3>Honors, Awards and Fellowships</h3>
<ul>
{% for award in site.data.awards %}
<li>{{ award.name }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

{% if site.data.achievements %}
<div class="section-card">
<h3>Achievements</h3>
<ul>
{% for item in site.data.achievements %}
<li>{{ item.name }}</li>
{% endfor %}
</ul>
</div>
{% endif %}

<div class="section-card">
<h3>Leadership and Extracurricular</h3>
<ul>
<li><strong>Deputy Contingent Leader</strong>, Inter-IIT Tech Meet 13.0, IIT (BHU) Contingent (2024). Led and coordinated a contingent of 90+ members across technical, managerial, and design problem statements; oversaw team selection, logistics, and practice schedules. The contingent secured two gold medals and a bronze.</li>
<li><strong>Captain</strong>, Table Tennis Club, IIT (BHU) (2024 &ndash; 2026). Captained the institute team at the home fest, out fest, and Inter-IIT Sports Meet; organized training and mentored junior players, contributing to gold, silver, and bronze medal finishes.</li>
</ul>
</div>

<div class="section-card">
<h3>Technical Skills</h3>
<ul>
<li><strong>Languages:</strong> C++ (proficient); Python, Julia, Rust, Go, TypeScript/JavaScript, Java, SQL</li>
<li><strong>ML / Scientific:</strong> PyTorch, scikit-learn, LLMs, NLP; SciML / DifferentialEquations.jl, JumpProcesses.jl, Molly.jl; DFT and electronic structure, molecular dynamics, cheminformatics (RDKit)</li>
<li><strong>Systems / Tools:</strong> CUDA and GPU kernels, Docker, Kubernetes, Git, Linux, AWS, CI/CD, Node.js, React, Flask, GraphQL, LaTeX</li>
</ul>
</div>
