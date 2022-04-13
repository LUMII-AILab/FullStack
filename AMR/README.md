# Abstract Meaning Representation

## Data

An automatically derived AMR annotation layer of the FullStack-LV multi-layer text corpus.

* First, Latvian UD Treebank (v2.5) sentences were translated to English using a state-of-the-art Latvian-English neural MT system ([Hugo.lv](https://hugo.lv/en)).
* Second, a state-of-the-art AMR parser for English ([AMREager](http://cohort.inf.ed.ac.uk/amreager.html)) was applied to the MT-translated sentences.
* Additionally, alignment information is provided for both Latvian-English translations and English-AMR parses.

## Data format

### Metadata

- `id` - the sentence ID according to the Latvian UD Treebank data.
- `snt_lv` - the original sentence (Latvian).
- `snt` - the machine-translated sentence (English).
- `alignments_translation` - token-level alignment between the Latvian and English sentences.
- `alignments` - alignment between tokens (English) and nodes of the AMR graph (see the [alignment format](https://github.com/lil-lab/amr/blob/07b581e7d160fa2625eeefa86ae5e9fe5c589be2/utils/jamr/docs/Alignment_Format.md)).


### AMR graph

The English translation encoded as an AMR graph in the PENMAN notation (see the [language specification](https://amr.isi.edu/language.html)).

Each record in the dataset is separated by an empty line. The dataset is split into subsets for training, development and testing using the same split as for the Latvian UD Treebank (v2.5).

### Example

```
# ::id a-p3315-p3s6
# ::snt Sister Ilze is also a model .
# ::snt_lv Māsa Ilze arī ir modelētāja.
# ::alignments 0-1|0.2+0.2.0+0.2.0.0 1-2|0.1+0.1.0+0.1.0.0 3-4|0.0 5-6|0
# ::alignments_translation 0-0 1-1 3-2 2-3 4-4 4-5 5-6
(v7 / modelētāja                           		-> 0
    :mod (v6 / also)                        		-> 0.0
    :domain (v4 / person                    		-> 0.1
        :name (v5 / name                    		-> 0.1.0
            :op1 "Ilze"))                    		-> 0.1.0.0
    :poss (v1 / person                      		-> 0.2
        :ARG0-of (v2 / have-rel-role-91     		-> 0.2.0
            :ARG2 (v3 / sister))))          		-> 0.2.0.0
```

- _Sister_: `(0-1) => v1+v2+v3 (0.2+0.2.0+0.2.0.0)`
- _Ilze_: `(1-2) => v4+v5+op1+wiki (0.1+0.1.0+0.1.0.0)`
- _also_: `(3-4) => v6 (0.0)`
- _model_: `(5-6) => v7`

## Current statistics

* __12,691__ whole-sentence AMR graphs
