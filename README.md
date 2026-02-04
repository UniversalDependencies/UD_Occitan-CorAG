# Summary
UD_Old_Occitan-CorAG (Corpus de l'Ancien Gascon) is a corpus of medieval legal texts in Gascon, a variety of Old Occitan. The texts were digitized from printed editions and subsequently manually annotated in Universal Dependencies (PoS, functions and some morphological features).

# Introduction

In October 2025, CorAG corpus contains six medieval texts: 

|Title                                         |Year       | Edition                 | Sentences| Tokens    |
| :------------------------------------------- |:--------: |:----------------------: | :------: | ----:     |
| Coutumes et Privilèges de l’Entre-Deux-Mers  | 1214-1342 | Lépicier 1861           | 344      | 11,978    |
| Coutume de Banières                          | 1251      |                         | 77       | 3,099     |
| Coutume de Banières                          | 1260      |                         | 33       | 1,699     |
| Charte des Boucheries d’Orthez               | 1270      |                         | 34       | 1,274     |
| Charte d’Herrère                             | 1278      |                         | 53       | 1,835     |
| Les Fors Anciens de Béarn                    | 1460      | Ourliac & Gilles 1990   | 750      | 26,795    |
| **Total**                                    |           |                         | **1,291**| **46,680**|

**Editions:**
Lépicier, Jules, 1861. « Coutumes et privilèges de l’Entre-Deux-Mers », _Archives historiques du département de la Gironde_, 101-130.
Ourliac, Paul & Gilles, Monique, 1990. _Les Fors anciens de Béarn_. Paris: Éditions du Centre National de la Recherche Scientifique.

Electronic editions of _Coutume de Banières_ (1251 and 1260), _Charte des Boucheries d'Orthez_ (1270) and _Charte d'Herrère_ were generously shared with us by Professor Martin Glessgen (University of Zurich). 

**Train/Dev/Test split**

| Set               | Sentences| Tokens    |
| :---------------- | :------: | ----:     |
| Train             |   912    |   32,606  |
| Dev               |   98     |   3,713   |
| Test              |   281    |   10,361  |
| **Total**         | **1,291**| **46,680**|

Please note that CorAG treebank is still under development. A campain of revision and morphological annotation is underway and new material is being added to the collection. The structure of the treebank is therefore likely to change in subsequent releases. Please do not hesitate to contact us if you have any questions, suggestions or comments.

# Annotation

The texts were digitized, segmented and subsequently automatically annotated with [HOPS](https://github.com/hopsparser/hopsparser) and [BertForDeprel](https://github.com/kirianguiller/BertForDeprel)) parsers using bootstrapping methodology ([Peng et al 2022](https://hal.science/hal-03846834/document)) on [ArboratorGrew](https://arborator.grew.fr/#/) software.

The texts are annotated in PoS and syntactic functions (Universal Dependencies), following, wherever possible, the guidelines for Modern Occitan ([Miletić, Aleksandra, Bras, Myriam, Esher, Louise, Sibille, Jean & Vergez-Couret, Marianne, 2020](https://hal.science/hal-04925754v1)).

In addition, in this release of the corpus, verbs and auxiliaries are annotated in verb forms (VerbForm): Inf (infinitive), Fin (conjugated) and Part (participle). Congujated forms are annotated in Person and Number.

Participles without dependents are annotated as adjectives but are also provided verbal morphological features.  Participles (whether tagged as VERB or ADJ) are annotated in Tense (Past, Pres or Fut), Gender (Masc or Fem) and Number (Plur or Sing).

Pronouns are annotated in type (PronType: Dem for demonstrative, Ind for indefinite, Prs for personal and Rel for relative). Reflexive and possessive pronouns are also tagged (Reflexive=Yes and Poss=Yes). 

# Acknowledgments
The corpus is part of Professor Pierre Larrivée's (University of Caen) [Senior membership project](https://www.iufrance.fr/les-membres-de-liuf/membre/2346-pierre-larrivee.html) with the Institut Universitaire de France.

Manual annotation was performed by Barbara Francioni and Natasha Romanova. Technical support by Rayan Ziane and Khensa Daoudi. Digitization by Christelle Violette. Project coordination by Natasha Romanova.

We thank Professor Martin Glessgen and his team at the University of Zurich (authors of the online resource [Documents linguistiques galloromans](https://gallrom.linguistik.uzh.ch/#/) for provinding us with their editions of the thirteenth-century texts included in the corpus.

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
