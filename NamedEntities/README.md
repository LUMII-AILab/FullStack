# Named Entities

## Data

* Format: a version of [CoNLL-2003](https://www.clips.uantwerpen.be/conll2003/ner/) on top of a subset of [CoNLL-U](http://universaldependencies.org/format.html)

* Fields: [ID, FORM, LEMMA, UPOS, XPOS, FEATS] + [BIOTAG<sub>1</sub>, BIOTAG<sub>2</sub>, WIKI<sub>1</sub>, WIKI<sub>2</sub>]
  - BIOTAG<sub>1</sub>, WIKI<sub>1</sub>: outer entity
  - BIOTAG<sub>2</sub>, WIKI<sub>2</sub>: inner entity

* Tagset: person, GPE, organization, location, event, product, time, money, entity

* Wikification: experimental

## Current statistics

* __3,947__ paragraphs (text units)

* __9,697__ outer entities:
  - 3,104 person
  - 2,031 GPE
  - 1,847 organization
  - 1,227 time
  - 677 location
  - 293 product
  - 259 event
  - 215 entity
  - 44 money

* __944__ inner entities:
  - 543 GPE
  - 154 organization
  - 129 location
  - 51 person
  - 28 time
  - 15 entity
  - 19 event
  - 4 product
  - 1 money

* __3,650__ Wikipedia links from ambiguous outer entities (38%)
* __526__ Wikipedia links from ambiguous inner entities (56%)
