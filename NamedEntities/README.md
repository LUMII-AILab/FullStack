# Named Entities

## Data

* Format: a version of [CoNLL-2003](https://www.clips.uantwerpen.be/conll2003/ner/) on top of a subset of [CoNLL-U](http://universaldependencies.org/format.html)

* Fields: [ID, FORM, LEMMA, UPOS, XPOS, FEATS] + [BIOTAG<sub>1</sub>, BIOTAG<sub>2</sub>, WIKI<sub>1</sub>, WIKI<sub>2</sub>]
  - BIOTAG<sub>1</sub>, WIKI<sub>1</sub>: outer entity
  - BIOTAG<sub>2</sub>, WIKI<sub>2</sub>: inner entity

* Tagset: person, GPE, organization, location, event, product, time, money, entity

* Wikification: experimental

## Current statistics

* 3,505 paragraphs (text units)

* 8,303 outer entities:
  - 2,802 person
  - 1,692 GPE
  - 1,554 organization
  - 988 time
  - 593 location
  - 238 product
  - 221 event
  - 186 entity
  - 29 money

* 771 inner entities:
  - 459 GPE
  - 133 organization
  - 98 location
  - 41 person
  - 18 time
  - 11 entity
  - 10 event
  - 1 product

* 2,860 Wikipedia links from outer entities (34%)
* 408 Wikipedia links from inner entities (53%)
