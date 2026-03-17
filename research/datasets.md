---
layout: overview
title: Datasets
---

# Datasets

All QANTA datasets are freely available for research use.

---

{% for ds in site.data.datasets %}

## {{ ds.name }}

{{ ds.description }}

{% if ds.splits %}

| Split | Download |
|---|---|
{% for split in ds.splits %}| {{ split.name }} | {% if split.url %}[Download]({{ split.url }}){% else %}—{% endif %} |
{% endfor %}
{% endif %}

{% if ds.paper_id %}{% assign paper = site.data.papers | where: "id", ds.paper_id | first %}{% if paper %}**Paper**: {{ paper.authors }} — [{{ paper.title }}]({{ paper.url }}) · {{ paper.venue }} {{ paper.year }}{% if ds.page %} · [Project page]({{ ds.page }}){% endif %}{% endif %}{% endif %}

{% if ds.code_url %}**Code**: [{{ ds.code_url | remove: "https://" }}]({{ ds.code_url }}){% endif %}
{% if ds.license %}**License**: {{ ds.license }}{% endif %}
{% if ds.notes %}*{{ ds.notes }}*{% endif %}

---
{% endfor %}
