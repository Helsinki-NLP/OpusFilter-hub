---
languages:
- es-cni
- es-aym
- es-bzd
- es-gn
- es-oto
- es-nah
- es-quy
- es-tar
- es-shp
- es-hch

corpora:
- AmericasNLP-2021
- GlobalVoices
- JHUBC
- Tatoeba
- Mexican constitution
- Bolivian constitution
- Peruvian constitution

tags:
- custom preprocessor
- custom filter
- multiple translations
---

# The Helsinki submission to the AmericasNLP shared task

Filtering configuration used in the University of Helsinki submission
for the AmericasNLP 2021 shared task.

Original source: https://github.com/Helsinki-NLP/americasnlp2021-st

## How to use

The pre-collected datasets from the data folder of the
https://github.com/Helsinki-NLP/americasnlp2021-st repository are
required.

Steps:

1) Install OpusFilter>=2.0.0

2) Create OpusFilter configuration using `processed_data` as work directory:

```
python create_opusfilter_config.py opusfilter.yaml processed_data
```

3) Run OpusFilter on the configuration:

```
PYTHONPATH=$PYTHONPATH:. opusfilter opusfilter.yaml
```
(PYTHONPATH added to include custom preprocessors in `create_opusfilter_config.py`.)

The filtered output files are in: `processed_data/[LANGUAGE]/dedup_filtered.[LANGCODE].gz`

See further examples in the Makefile.

## BibTeX entry and citation info

```bibtex
@inproceedings{vazquez-etal-2021-helsinki,
    title = "The {H}elsinki submission to the {A}mericas{NLP} shared task",
    author = {V{\'a}zquez, Ra{\'u}l  and
      Scherrer, Yves  and
      Virpioja, Sami  and
      Tiedemann, J{\"o}rg},
    booktitle = "Proceedings of the First Workshop on Natural Language Processing for Indigenous Languages of the Americas",
    month = jun,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.americasnlp-1.29",
    doi = "10.18653/v1/2021.americasnlp-1.29",
    pages = "255--264",
}
```
