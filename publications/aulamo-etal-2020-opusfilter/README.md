---
languages:
- fi-en

corpora:
- ParaCrawl

tags:
- classifier
---

# OpusFilter experiments using ParaCrawl

Corpus filtering and domain adaptation experiments for Finnish-English
translation using ParaCrawl v4.

Original source: https://github.com/Helsinki-NLP/OpusFilter

## How to use

Run `opusfilter` on the configuration files in the following order:

- `prepare_data.yaml`
- `create_ce_sets.yaml`
- `create_roc_auc_sets.yaml`
- `create_domain_sets.yaml`
  - requires additional datasets, see comments in the file

## BibTeX entry and citation info

```bibtex
@inproceedings{aulamo-etal-2020-opusfilter,
    title = "{O}pus{F}ilter: A Configurable Parallel Corpus Filtering Toolbox",
    author = {Aulamo, Mikko and Virpioja, Sami and Tiedemann, J{\"o}rg},
    booktitle = "Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
    month = jul,
    year = "2020",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2020.acl-demos.20",
    doi = "10.18653/v1/2020.acl-demos.20",
    pages = "150--156",
}
```
