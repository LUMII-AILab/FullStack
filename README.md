# Full Stack of Latvian Language Resources for NLU and NLG

## Introduction

This repository contains a work-in-progress data set - a multilayer text corpus of Latvian. The broad application area we address is natural language understanding (NLU) and generation (NLG), and the aim of the corpus creation is to develop a data-driven NLU and NLG toolchain for Latvian. Both the multilayered corpus and the downstream applications are anchored in cross-lingual state-of-the-art representations: [Universal Dependencies](http://universaldependencies.org/) (UD), [FrameNet](https://framenet.icsi.berkeley.edu/fndrupal/), [PropBank](https://propbank.github.io/) and [Abstract Meaning Representation](https://amr.isi.edu/) (AMR). A complementary representation, language resource and technology for NLG, which is being developed separately, is [Grammatical Framework](http://www.grammaticalframework.org/) (GF).

The UD representation is automatically derived from a more elaborated and manually annotated [hybrid dependency-constituency representation](http://sintakse.korpuss.lv/).
The FrameNet annotations are manually added, guided by the underlying UD annotations. Consequently, frame elements are represented by the root nodes of the respective subtrees instead of text spans; the spans can be easily calculated from the subtrees.
The PropBank layer is automatically derived from the FrameNet and UD annotations, provided a manual mapping from FrameNet lexical units to PropBank frames, and a mapping from FrameNet frame elements to PropBank semantic roles for the given pair of FrameNet and PropBank frames.
Draft AMR graphs are to be derived from the UD and PropBank layers, as well as auxiliary layers containing named entity and coreference annotation. The semantically rich FrameNet annotations are also helpful in acquiring more accurate AMR graphs.

We are aiming at a medium-sized corpus: 10-15 thousand sentences annotated at all layers. Therefore it is important to ensure that the multilayer corpus is balanced not only in terms of text genres and writing styles but also in terms of lexical units.
A fundamental design decision is that the text unit is an isolated paragraph. The multilayer corpus therefore consists of manually selected paragraphs from many different texts of various types. Representative paragraphs are selected in different proportions from a balanced 10-million-word text corpus: 60% news sources, 20% fiction, 10% legal texts, 5% spoken language, 5% miscellaneous.

As for the lexical units, our goal is to cover 1,000-2,000 most frequently occurring verbs, calculated from the 10-million-word corpus. Since the most frequent verbs tend to be the most polysemous, we expect that the number of lexical units (verb senses w.r.t. semantic frames) will be considerably larger. We assume that the corpus will turn out to be rather balanced also w.r.t. nominal lexical units.

## Annotation layers

![Layers](fullstack.png)

## Publications

Normunds Gruzitis, Lauma Pretkalnina, Baiba Saulite, Laura Rituma, Gunta Nespore-Berzkalne, Arturs Znotins, Peteris Paikens. [Creation of a balanced state-of-the-art multilayer corpus for NLU](http://www.lrec-conf.org/proceedings/lrec2018/pdf/935.pdf). Proceedings of the 11th International Conference on Language Resources and Evaluation (LREC), 2018, pp. 4506-4513

Normunds Gruzitis, Gunta Nespore-Berzkalne, Baiba Saulite. [Creation of Latvian FrameNet based on Universal Dependencies](http://lrec-conf.org/workshops/lrec2018/W5/pdf/9_W5.pdf). Proceedings of the International FrameNet Workshop 2018: Multilingual FrameNets and Constructicons (IFNW), 2018, pp. 23-27

Normunds Gruzitis, Didzis Gosko, Guntis Barzdins. [RIGOTRIO at SemEval-2017 Task 9: Combining machine learning and grammar engineering for AMR parsing and generation](http://www.aclweb.org/anthology/S17-2159). Proceedings of the 11th International Workshop on Semantic Evaluation (SemEval), 2017, pp. 924-928

## Acknowledgements

This work is supported by the European Regional Development Fund under the grant agreements No. 1.1.1.1/16/A/219 (*Full Stack of Language Resources for Natural Language Understanding and Generation in Latvian*) and No. 1.1.1.2/VIAA/1/16/188 (*From Abstract Meaning Representation to Natural Language Sentence and Coherent Text Generation*).

## Licence

This data set by [AiLab](http://ailab.lv) is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). Please contact us if you are interested in acquiring a commercial licence.

## Contacts

Coordinator of the project: [Normunds Grūzītis](https://www.linkedin.com/in/normundsg), `normunds.gruzitis@ailab.lv`

Team members: Ilze Auziņa, Guntis Bārzdiņš, Roberts Darģis, Mikus Grasmanis, Kristīne Levāne-Petrova, Gunta Nešpore-Bērzkalne, Pēteris Paikens, Lauma Pretkalniņa, Laura Rituma, Inguna Skadiņa, Baiba Valkovska (Saulīte), Artūrs Znotiņš
