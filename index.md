---
layout: home
title: Home
explore:
  - title: "2026 Competition"
    url: /competition/2026/
    text: "The world's first multimodal Quizbowl competition — text and image clues. Compete, write questions, or build a multimodal AI system."
    badges:
      - label: "Coming 2026"
        class: badge-danger
  - title: Research
    url: /research/
    text: "Projects and datasets spanning adversarial QA, sequential reasoning, conversational contexts, and knowledge graph QA."
    badges:
      - label: "4 Projects"
        class: badge-secondary
      - label: "5 Datasets"
        class: badge-secondary
  - title: "Data &amp; Code"
    url: /data-and-code/
    text: "Download QANTA datasets and explore open-source code on GitHub. Evaluate your system on CodaLab."
    badges:
      - label: "Open Source"
        class: badge-secondary
---

<section class="py-2">
<h2 class="mt-0">What is QANTA?</h2>

The QANTA project uses trivia competitions to compare computer systems against expert humans in games of question answering. Our goal is to advance question answering — helping computers learn from how trivia experts think, studying human–computer collaboration, and building tools that help humans write challenging questions efficiently.

Led by **[Jordan Boyd-Graber]({{ site.pi.url }})** (University of Maryland), QANTA brings together researchers from computer science, linguistics, and information science at UMD and UC Berkeley.
</section>

<section class="py-4 px-4 my-2 section-card">
<h2 class="mt-0">Explore</h2>
<div class="row mt-3">
{%- for card in page.explore %}<div class="col-md-4 mb-3"><div class="card h-100 card-accent shadow-sm"><div class="card-body"><h5 class="card-title"><a href="{{ card.url }}" class="stretched-link text-decoration-none text-dark">{{ card.title }}</a></h5><p class="card-text text-muted">{{ card.text }}</p>{% for b in card.badges %}<span class="badge {{ b.class }}">{{ b.label }}</span>{% endfor %}</div></div></div>
{%- endfor %}</div>
</section>

<section class="py-4">
<h2>In the News</h2>
<div class="mt-3">
{%- for item in site.data.news %}<div class="news-item"><span class="news-year">{{ item.year }}</span>{% if item.url %}<a href="{{ item.url }}">{{ item.text }}</a>{% elsif item.html %}{{ item.html }}{% else %}{{ item.text }}{% endif %}</div>
{%- endfor %}</div>
</section>

<section class="py-3">
<h2>Contact</h2>

Questions about QANTA? Email **[{{ site.contact_email }}](mailto:{{ site.contact_email }})** or reach out to [Jordan Boyd-Graber](mailto:{{ site.pi.email }}) directly. Website maintained by the QANTA team.
</section>
