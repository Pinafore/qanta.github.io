---
layout: overview
title: Data & Code
---

# Data & Code

All QANTA datasets and code are freely available for research use.

---

## GitHub Repositories

| Repository | Description |
|---|---|
| [Pinafore/qb]({{ site.github.main }}) | Main QA system used in exhibition matches — large, actively developed |
| [Pinafore/qanta-codalab]({{ site.github.codalab }}) | Simplified system designed for inspection, extension, and leaderboard submission |
| [aagohary/canard](https://github.com/aagohary/canard) | CANARD question-rewriting code, data, and OpenNMT baseline |
| [henryzhao5852/DELFT](https://github.com/henryzhao5852/DELFT) | DELFT system code and Wikipedia graph data |

---

## Datasets

| Dataset | Description | Download |
|---|---|---|
{% for ds in site.data.datasets %}| {% if ds.page %}[{{ ds.short_name }}]({{ ds.page }}){% else %}{{ ds.short_name }}{% endif %} | {{ ds.description | truncatewords: 15 }} | {% assign dl_splits = ds.splits | where_exp: "s", "s.url" %}{% if dl_splits.size > 0 %}{% for split in dl_splits %}[{{ split.name }}]({{ split.url }}){% unless forloop.last %} · {% endunless %}{% endfor %}{% else %}[Contact us](mailto:{{ site.contact_email }}){% endif %} |
{% endfor %}

See the [Datasets page](/research/datasets/) for full descriptions and citation information.

---

## Leaderboard

Submit your system to the **[CodaLab leaderboard](https://codalab.lisn.upsaclay.fr/)**. Example worksheets and baseline submissions are available in [Pinafore/qanta-codalab]({{ site.github.codalab }}).

---

## Contact

For dataset access or questions: [{{ site.contact_email }}](mailto:{{ site.contact_email }})
