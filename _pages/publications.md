---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">
<h2>Refereed Journal Articles</h2>

{% bibliography --query @article %}

<h2>Preprints and Manuscripts</h2>

{% bibliography --query @misc %}

{% bibliography --query @unpublished %}
</div>

<p class="text-muted">A full list is also available on <a href="{{ site.links.google_scholar }}">Google Scholar</a>.</p>
