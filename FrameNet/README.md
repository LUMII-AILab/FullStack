# FrameNet

## Data

A manually annotated Latvian FrameNet annotation layer of the [FullStack](https://github.com/LUMII-AILab/FullStack) corpus.

* __Format__: a version of [CoNLL-2009](http://ufal.mff.cuni.cz/conll2009-st/task-description.html) on top of [CoNLL-U](http://universaldependencies.org/format.html)

* __Fields__: [ID, FORM, LEMMA, UPOS, XPOS, FEATS, HEAD, DEPREL, DEPS] + [FILLPRED, PRED, APRED]
  - FILLPRED: indicates the target word
  - PRED: semantic frame
  - APRED: frame elements

__Note__ that each corpus example contains one FrameNet annotation set (frame instance). If there are several annotation sets for the same sentence, they are included as separate corpus examples.

## Current statistics

* Annotation sets: __10,952__
* Semantic frames: __458__
* Lexical units: __1,658__
* Target words (lexemes): __863__
