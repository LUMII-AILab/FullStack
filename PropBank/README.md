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

* [_Mapping_] Target verbs: __1,322__ out of 1,358 (97.3%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
* [_Mapping_] FrameNet frames: __521__ out of 540 (96.5%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
* [_Mapping_] FrameNet lexical units: __2,377__ out of 2,577 (92.2%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
* [_Mapping_] PropBank predicates: __1,033__ out of 10,687 (9.7%) - cf. [English PropBank](https://propbank.github.io/)
* [_Data_] Annotation sets: __20,054__ out of 20,879 (96.0%) - cf. [Latvian FrameNet](https://github.com/LUMII-AILab/FullStack/tree/master/FrameNet)
