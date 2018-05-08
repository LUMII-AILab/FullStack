# Named Entities

## Data

* Format: a version of [CoNLL-2003](https://www.clips.uantwerpen.be/conll2003/ner/) on top of a subset of [CoNLL-U](http://universaldependencies.org/format.html)

* Fields: [ID, FORM, LEMMA, UPOSTAG, XPOSTAG, FEATS] + [BIOTAG<sub>1</sub>, BIOTAG<sub>2</sub>, WIKI<sub>1</sub>, WIKI<sub>2</sub>]
  - BIOTAG<sub>1</sub>, WIKI<sub>1</sub>: outer entity
  - BIOTAG<sub>2</sub>, WIKI<sub>2</sub>: inner entity

* Tagset: person, GPE, organization, location, event, product, time, entity

* Wikification: experimental

## Current statistics

* 2,097 paragraphs (text units)

* 4,281 outer entities:
  - 1,540 person
  - 975 organization
  - 734 GPE
  - 478 time
  - 277 location
  - 101 product
  - 96 entity
  - 80 event

* 388 inner entities:
  - 219 GPE
  - 90 organization
  - 38 location
  - 19 person
  - 10 time
  - 8 entity
  - 3 event
  - 1 product

* 820 Wikipedia links from outer entities (19%)
* 116 Wikipedia links from inner entities (30%)
