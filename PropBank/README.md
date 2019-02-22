# PropBank

## Mapping

A mapping configuration from lexical units in [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet) to [PropBank](https://propbank.github.io/) frames, and a mapping configuration from [FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/) frame elements and their [UD](http://universaldependencies.org/) roles in [Latvian UD Treebank](https://github.com/LUMII-AILab/FullStack/tree/master/UD) roles to PropBank semantic roles for the given pair of FrameNet and PropBank frames.

## Data

An automatically derived Latvian PropBank annotation layer of the FullStack corpus: work in progress.

* Format: a version of [CoNLL-2009](http://ufal.mff.cuni.cz/conll2009-st/task-description.html) on top of [CoNLL-U](http://universaldependencies.org/format.html)

* Fields: [ID, FORM, LEMMA, UPOS, XPOS, FEATS, HEAD, DEPREL, DEPS] + [FILLPRED, PRED, APRED<sub>1</sub>, ..., APRED<sub>n</sub>]
  - PRED: semantic frames
  - APRED: semantic roles

## Current statistics

Coverage:

* Target verbs: 459 out of 835 (55%)
* FrameNet frames: 182 out of 452 (40%)
* FrameNet lexical units (verb-frame pairs): 575 out of 1,575 (37%)
* PropBank frames (predicates): 353
* Annotation sets (corpus examples): 2,861 out of 7,371 (39%)
