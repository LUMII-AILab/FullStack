# FrameNet

## Data

A manually created Latvian FrameNet annotation layer of the [FullStack](https://github.com/LUMII-AILab/FullStack) multi-layer text corpus.

* __Format__: a version of [CoNLL-2009](http://ufal.mff.cuni.cz/conll2009-st/task-description.html) on top of [CoNLL-U](http://universaldependencies.org/format.html)

* __Fields__: [ID, FORM, LEMMA, UPOS, XPOS, FEATS, HEAD, DEPREL, DEPS] + [FILLPRED, PRED, APRED]
  - FILLPRED: indicates the target word
  - PRED: semantic frame
  - APRED: frame elements

__Note__ that each corpus example (a whole sentence) contains one FrameNet annotation set (a frame instance). If there are several annotation sets for the same sentence, they are included as separate corpus examples.

## Evaluation data

A subset of the complete Latvian FrameNet dataset, where:
* For each lexical unit (LU), 80% of the annotation sets are included in the training dataset, and 20% - in the test dataset.
* Only LUs having at least 10 annotation sets (at least 8 training examples and at least 2 test examples) are considered and included in the evaluation dataset.

## Current statistics

* Annotation sets: __20,879__
* Semantic frames (Berkeley FrameNet): __540__
* Lexical units (word-frame pairs): __2,577__
* Target words (lexemes): __1,358__
