# PropBank

## Mapping

A mapping configuration from lexical units (verb-frame pairs) in [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet) to [English PropBank](https://propbank.github.io/) predicates, and a mapping configuration from [FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/) frame elements and their [Universal Dependencies](http://universaldependencies.org/) relations in [Latvian UD Treebank](https://github.com/LUMII-AILab/FullStack/tree/master/UD) to PropBank semantic roles for the given pair of a FrameNet frame and a PropBank predicate.

## Data

An automatically derived Latvian PropBank annotation layer of the [FullStack](https://github.com/LUMII-AILab/FullStack) multi-layer text corpus. PropBank annotations are derived based on the mapping configuration.

* __Format__: compliant to [Universal Propositions](https://github.com/System-T/UniversalPropositions), which is based on [CoNLL-U](http://universaldependencies.org/format.html) and is extended with [CoNLL-2009](http://ufal.mff.cuni.cz/conll2009-st/task-description.html)-style semantic role labeling annotations.

* __Fields__: [ID, FORM, LEMMA, UPOS, XPOS, FEATS, HEAD, DEPREL] + [FILLPRED, PRED, APRED]
  - FILLPRED: indicates the target word
  - PRED: semantic frame
  - APRED: semantic roles

__Note__ that each corpus example contains one PropBank annotation set. If there are several annotation sets for the same sentence, they are included as separate corpus examples.

## Current statistics

* [_Mapping_] Target verbs: __986__ out of 1,358 (73%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
* [_Mapping_] FrameNet frames: __440__ out of 540 (82%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
* [_Mapping_] FrameNet lexical units: __1,657__ out of 2,577 (64%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
* [_Mapping_] PropBank predicates: __795__ out of 7,311 (11%) - cf. [English PropBank](https://propbank.github.io/)
* [_Data_] Annotation sets: __17,015__ out of 20,879 (82%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
