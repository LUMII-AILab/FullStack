# Named Entities

## Data

* Format: a version of [CoNLL-2003](https://www.clips.uantwerpen.be/conll2003/ner/) on top of a subset of [CoNLL-U](http://universaldependencies.org/format.html)

* Fields: [ID, FORM, LEMMA, UPOS, XPOS, FEATS] + [BIOTAG<sub>1</sub>, BIOTAG<sub>2</sub>, WIKI<sub>1</sub>, WIKI<sub>2</sub>]
  - BIOTAG<sub>1</sub>, WIKI<sub>1</sub>: outer entity
  - BIOTAG<sub>2</sub>, WIKI<sub>2</sub>: inner entity

* Tagset: person, GPE, organization, location, event, product, time, entity

* Wikification: experimental

## Current statistics

* 2,833 paragraphs (text units)

* 6,362 outer entities:
  - 2,072 person
  - 1,335 GPE
  - 1,297 organization
  - 733 time
  - 452 location
  - 167 entity
  - 155 product
  - 151 event

* 575 inner entities:
  - 328 GPE
  - 116 organization
  - 72 location
  - 29 person
  - 14 time
  - 10 entity
  - 5 event
  - 1 product

* 1,903 Wikipedia links from outer entities (30%)
* 250 Wikipedia links from inner entities (43%)
