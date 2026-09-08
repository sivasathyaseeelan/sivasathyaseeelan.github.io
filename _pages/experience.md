---
title: "Experience"
layout: page
permalink: /experience/
---

# Experience

{% assign groups = "research,work" | split: "," %}
{% for g in groups %}
{% assign entries = site.data.experience[g] %}
{% if entries.size > 0 %}
<h2>{% if g == "research" %}Research Experience{% else %}Work Experience{% endif %}</h2>

{% for e in entries %}
<div class="section-card" markdown="0">
<div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: baseline; gap: var(--space-2);">
<h3 style="margin: 0;">{{ e.role }}</h3>
<span class="year-badge">{{ e.period }}</span>
</div>
<p style="margin: var(--space-2) 0 0; font-style: italic; color: var(--text-secondary);">{% if e.url %}<a href="{{ e.url }}" target="_blank">{{ e.org }}</a>{% else %}{{ e.org }}{% endif %}{% if e.location %} &middot; {{ e.location }}{% endif %}{% if e.advisor %} &middot; Advisor: {% if e.advisor_url %}<a href="{{ e.advisor_url }}" target="_blank">{{ e.advisor }}</a>{% else %}{{ e.advisor }}{% endif %}{% endif %}</p>
{% if e.bullets %}
<ul style="margin-top: var(--space-3);">
{% for b in e.bullets %}<li>{{ b }}</li>
{% endfor %}
</ul>
{% endif %}
{% if e.tags %}<p class="text-muted" style="margin: 0; font-size: 0.9rem;"><strong>Exposure:</strong> {{ e.tags }}</p>{% endif %}
</div>
{% endfor %}
{% endif %}
{% endfor %}
