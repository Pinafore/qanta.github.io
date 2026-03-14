---
layout: overview
title: Research
---

# Research

QANTA investigates question answering at the intersection of natural language processing, human–computer interaction, and machine learning. Our work spans dataset creation, system building, and competition design.

## Areas

<div class="row mt-3 mb-4">
  <div class="col-md-6 mb-3">
    <div class="card shadow-sm h-100">
      <div class="card-body">
        <h5 class="mt-0"><a href="/research/projects/">Projects</a></h5>
        <p class="mb-0">Individual research efforts with papers, code, and data — from adversarial question writing to graph-based QA systems.</p>
      </div>
    </div>
  </div>
  <div class="col-md-6 mb-3">
    <div class="card shadow-sm h-100">
      <div class="card-body">
        <h5 class="mt-0"><a href="/research/datasets/">Datasets</a></h5>
        <p class="mb-0">Quiz bowl corpora and specialized QA benchmarks, freely available for research. Includes real download links.</p>
      </div>
    </div>
  </div>
</div>

## Selected Publications

| Paper | Authors | Venue |
|---|---|---|
{% for paper in site.data.papers %}| {% if paper.url %}[{{ paper.title }}]({{ paper.url }}){% else %}{{ paper.title }}{% endif %} | {{ paper.authors }} | {{ paper.venue }} {{ paper.year }} |
{% endfor %}

## Principal Investigator

**[Jordan Boyd-Graber](http://users.umiacs.umd.edu/~jbg/)** — University of Maryland, College Park. Research interests: machine learning, probabilistic graphical models, and their applications in natural language processing.
