# Summary
UD_Old_Occitan-CorAG (Corpus de l'Ancien Gascon) is a corpus of medieval and early modern legal texts in Gascon, a variety of Old Occitan. The texts were digitized from existing editions and subsequently manually annotated in Universal Dependencies (PoS, functions and some morphological features).

# Introduction

In May 2025, CorAG corpus contains six medieval texts and a section of a sixteenth-century text: 


|Title                                         | Year      |Code            | Edition                | 
| :-------------------------------------------:|:--------: |:-------------: | :---------------------:|
| Coutumes et Privilèges de l’Entre-Deux-Mers  | 1214-1342 | 1214-1342_Deux |Lépicier 1861           | 
| Coutume de Banières                          | 1251      | 1251_Bagn      |Maldonado 2022          | 
| Coutume de Banières                          | 1260      | 1260_Bagn      |Maldonado 2022          | 
| Charte des Boucheries d’Orthez               | 1270      | 1270_Orthez    |Glessgen 2022           | 
| Charte d’Herrère                             | 1278      | 1278_Herr      |Glessgen (unpublished)  | 
| Les Fors Anciens de Béarn                    | 1460      | 1460_Bearn     |Ourliac & Gilles 1990   |
| Stil de la justicy (partial)                 | 1564      | 1564_Stil      |Ravier 1663             |


# Editions:
Lépicier, Jules, 1861. « Coutumes et privilèges de l’Entre-Deux-Mers », _Archives historiques du département de la Gironde_, 101-130.
Ourliac, Paul & Gilles, Monique, 1990. _Les Fors anciens de Béarn_. Paris: Éditions du Centre National de la Recherche Scientifique.

Electronic editions of _Coutume de Banières_ (1251 and 1260), _Charte des Boucheries d'Orthez_ (1270) and _Charte d'Herrère_ were generously shared with the CorAG team by Professor Martin Glessgen (University of Zurich). 

# Train/Dev/Test split

| Source | Train (sent) | Train (tok) | Dev (sent) | Dev (tok) | Test (sent) | Test (tok) | Total (sent) | Total (tok) |
|--------|--------------|-------------|------------|-----------|-------------|------------|--------------|-------------|
| 1214-1342_Deux | 244 | 8,418 | 21 | 964 | 78 | 2,249 | 343 | **11,631** |
| 1251_Bagn | 53 | 2,185 | 8 | 248 | 17 | 589 | 78 | **3,022** |
| 1260_Bagn | 22 | 1,082 | 4 | 169 | 7 | 409 | 33 | **1,660** |
| 1270_Orthez | 24 | 907 | 4 | 151 | 6 | 282 | 34 | **1,340** |
| 1278_Herr | 36 | 1,245 | 6 | 182 | 11 | 355 | 53 | **1,782** |
| 1460_Bearn | 576 | 18,901 | 58 | 2,102 | 119 | 4,951 | 753 | **25,954** |
| 1564_Stil | 137 | 5,188 | 17 | 589 | 38 | 1,372 | 192 | **7,149** |
| Total | 1092 | 37,926 | 118 | 4,405 | 276 | 10,207 | 1486 | **52,538** |

| Split | Sentences | Tokens | % (tokens) |
|-------|-----------|--------|------------|
| train | 1,092 | 37,926 | 72.2% |
| dev | 118 | 4,405 | 8.4% |
| test | 276 | 10,207 | 19.4% |
| Total | 1,486 | 52,538 | 100.0% |

Please note that CorAG treebank is still under development. A campain of revision and morphological annotation is underway and new material is being added to the collection. The structure of the treebank is therefore likely to change in subsequent releases. Please do not hesitate to contact us if you have any questions, suggestions or comments.

# Annotation

The texts were digitized, segmented and subsequently automatically annotated with [HOPS](https://github.com/hopsparser/hopsparser) and [BertForDeprel](https://github.com/kirianguiller/BertForDeprel)) parsers using bootstrapping methodology ([Peng et al 2022](https://hal.science/hal-03846834/document)) on [ArboratorGrew](https://arborator.grew.fr/#/) software.

The texts are annotated in PoS and syntactic functions (Universal Dependencies), following, wherever possible, the guidelines for Modern Occitan ([Miletić, Aleksandra, Bras, Myriam, Esher, Louise, Sibille, Jean & Vergez-Couret, Marianne, 2020](https://hal.science/hal-04925754v1)).

In addition, in this release of the corpus, verbs and auxiliaries are annotated in verb forms (VerbForm): Inf (infinitive), Fin (conjugated) and Part (participle). Congujated forms are annotated in Person and Number.

Participles without dependents are annotated as adjectives but are also provided verbal morphological features.  Participles (whether tagged as VERB or ADJ) are annotated in Tense (Past, Pres or Fut), Gender (Masc or Fem) and Number (Plur or Sing).

Pronouns are annotated in type (PronType: Dem for demonstrative, Ind for indefinite, Prs for personal and Rel for relative). Reflexive and possessive pronouns are also tagged (Reflexive=Yes and Poss=Yes). 

# Acknowledgments
The corpus is part of Professor Pierre Larrivée's (University of Caen) [Senior membership project](https://www.iufrance.fr/les-membres-de-liuf/membre/2346-pierre-larrivee.html) with the Institut Universitaire de France.

Manual annotation was performed by [Barbara Francioni](https://cv.hal.science/barbara-francioni) and [Natasha Romanova](https://cv.hal.science/natasha-romanova). Technical support by [Rayan Ziane](https://cv.hal.science/rayan-ziane) and Khensa Daoudi. Digitization by Christelle Violette. Project coordination by Natasha Romanova.

We thank Professor Martin Glessgen and his team at the University of Zurich (authors of the online resource [Documents linguistiques galloromans](https://gallrom.linguistik.uzh.ch/#/) for provinding us with their editions of the thirteenth-century texts included in the corpus.

The version of the treebank from November 2025 can also be consulted via the CRISCO Lab (University of Caen) [TXM portal](https://txm-crisco.huma-num.fr/txm/).

We thank the members of the Modern Occitan [Tolosa Treebank](https://github.com/UniversalDependencies/UD_Occitan-TTB) for their help and advice in the early stages of the annotation process.

## References
To cite the corpus, please refer to:
* Romanova, Natasha, Ziane, Rayan & Francioni, Barbara, 2025. « Adaptation of models for parsing of Old Gascon ». _Proceedings of Journées scientifiques du réseau thématique LIFT2 linguistique informatique, formelle et de terrain_. 16-17 October 2025, Paris. URL: https://lift2-2025.sciencesconf.org/667164 (8pp.)

See also:
* Daoudi, Khensa, Dehouck, Mathieu, Romanova, Natasha & Ziane, Rayan, 2025. « Explicit Edge Length Coding to Improve Long Sentence Parsing Performance ». _Proceedings of the First Workshops on Advancing NLP for Low-Resource Languages_. 13 September 2025, Varna, Bulgaria. URL: https://acl-bg.org/proceedings/2025/LowResNLP%202025/index.html (pp. 102-110)


# Changelog

* 2025-11-15 v2.17
  * Repository renamed from UD_Occitan-CorAG to UD_Old_Occitan-CorAG.
* 2025-05-15 v2.16
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.16
License: CC BY-SA 4.0
Includes text: yes
Parallel: no
Genre: legal
Lemmas: automatic
UPOS: manual native
XPOS: not available
Features: not available
Relations: manual native
Contributors: Francioni, Barbara; Romanova, Natalia; Ziane, Rayan; Daoudi, Khensa; Larrivée, Pierre
Contributing: here
Contact: natalia.romanova@unicaen.fr
===============================================================================
</pre>
