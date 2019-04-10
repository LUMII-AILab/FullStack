# PropBank

## Mapping

A mapping configuration from lexical units in [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet) to [PropBank](https://propbank.github.io/) frames, and a mapping configuration from [FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/) frame elements and their [UD](http://universaldependencies.org/) roles in [Latvian UD Treebank](https://github.com/LUMII-AILab/FullStack/tree/master/UD) roles to PropBank semantic roles for the given pair of FrameNet and PropBank frames.

## Data

An automatically derived Latvian PropBank annotation layer of the [FullStack](https://github.com/LUMII-AILab/FullStack) corpus. PropBank annotations are derived based on the mapping configurations.

* __Format__: compliant to [Universal Propositions](https://github.com/System-T/UniversalPropositions), which is based on [CoNLL-U](http://universaldependencies.org/format.html) and is extended with [CoNLL-2009](http://ufal.mff.cuni.cz/conll2009-st/task-description.html)-style semantic role labeling annotations.

* __Fields__: [ID, FORM, LEMMA, UPOS, XPOS, FEATS, HEAD, DEPREL] + [FILLPRED, PRED, APRED]
  - FILLPRED: indicates the target word
  - PRED: semantic frame
  - APRED: semantic roles

__Note__ that each corpus example contains one PropBank annotation set. If there are several annotation sets for the same sentence, they are included as separate corpus examples.

## Current statistics

* [_Mapping_] Target verbs: __554__ out of 835 (66%)
* [_Mapping_] FrameNet frames: __239__ out of 452 (53%)
* [_Mapping_] FrameNet lexical units (verb-frame pairs): __746__ out of 1,575 (47%)
* [_Mapping_] PropBank frames (predicates): __438__ out of 7,311 (6%)
* [_Data_] Annotation sets: __3,613__ out of 7,371 (49%)
