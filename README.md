# Summary
UD_Old_Occitan-CorAG (Corpus de l'Ancien Gascon) is a corpus of medieval and early modern legal texts in Gascon, a variety of Old Occitan. The texts were digitized from existing editions and subsequently manually annotated in Universal Dependencies (PoS, functions and some morphological features).

# Introduction

In May 2026, CorAG corpus contains six medieval texts and a section of a sixteenth-century text: 


|Title                                         | Year      |Code            | Edition                | 
| :-------------------------------------------:|:--------: |:-------------: | :---------------------:|
| Coutumes et Privilèges de l’Entre-Deux-Mers  | 1214-1342 | 1214-1342_Deux |Lépicier 1861           | 
| Coutume de Banières                          | 1251      | 1251_Bagn      |Maldonado 2022          | 
| Coutume de Banières                          | 1260      | 1260_Bagn      |Maldonado 2022          | 
| Charte des Boucheries d’Orthez               | 1270      | 1270_Orthez    |Glessgen 2022           | 
| Charte d’Herrère                             | 1278      | 1278_Herr      |Glessgen (unpublished)  | 
| Les Fors Anciens de Béarn                    | 1460      | 1460_Bearn     |Ourliac & Gilles 1990   |
| Stil de la justicy (partial)                 | 1564      | 1564_Stil      |Rovier 1663             |


# Editions
Lépicier, Jules, 1861. « Coutumes et privilèges de l’Entre-Deux-Mers », _Archives historiques du département de la Gironde_, pp. 101-130.

Glessgen, Martin, 2022. L’étude linguistique du gascon médiéval : analyse scriptologique des genres textuels, _Revue de linguistique romane_ 86, 35 - 94.

Maldonado, Lucas, 2022. _Les documents gascons originaux du XIII<sup>e</sup> siècle: éditions et analyses linguistiques_. Master's Dissertation. Sorbonne Université.

Ourliac, Paul & Gilles, Monique, 1990. _Les Fors anciens de Béarn_. Paris: Éditions du Centre National de la Recherche Scientifique.

Rovier, Jacques, 1663. _Stil de la justicy deu pais de Bearn_. Orthez.

The latest versions of the electronic editions of _Coutume de Banières_ (1251 and 1260), _Charte des Boucheries d'Orthez_ (1270) and _Charte d'Herrère_ were generously shared with the CorAG team by Professor Martin Glessgen and his team (University of Zurich) in 2023. 

# Corpus stats

| File | Sentences | Tokens (synt) | Tokens (surf) | Tokens+MWT | MWT | Empty | Forms (uniq) | Lemmas (uniq) | UPOS | Avg sent len | Min | Max |
|------|-----------|---------------|---------------|------------|-----|-------|--------------|---------------|------|--------------|-----|-----|
| 1214-1342_Deux | 343 | 11,632 | 11,333 | 11,931 | 299 | 0 | 2,314 | 0 | 14 | 33.9 | 3 | 178 |
| 1251_Bagn | 78 | 3,022 | 2,810 | 3,234 | 212 | 0 | 657 | 0 | 14 | 38.7 | 5 | 147 |
| 1260_Bagn | 33 | 1,660 | 1,557 | 1,763 | 103 | 0 | 514 | 0 | 14 | 50.3 | 11 | 250 |
| 1270_Orthez | 34 | 1,340 | 1,303 | 1,377 | 37 | 0 | 395 | 0 | 14 | 39.4 | 8 | 169 |
| 1278_Herr | 53 | 1,782 | 1,726 | 1,838 | 56 | 0 | 518 | 0 | 13 | 33.6 | 10 | 130 |
| 1460_Bearn | 753 | 25,954 | 25,357 | 26,551 | 597 | 0 | 2,946 | 0 | 13 | 34.5 | 3 | 332 |
| 1564_Stil | 192 | 7,149 | 6,942 | 7,356 | 207 | 0 | 1,536 | 0 | 13 | 37.2 | 6 | 187 |
| Total | 1,486 | 52,539 | 51,028 | 54,050 | 1,511 | 0 | — | — | — | 35.4 | — | — |

# Train/Dev/Test split

| File | Sentences | Tokens (synt) | Tokens (surf) | Tokens+MWT | MWT | Empty | Forms (uniq) | Lemmas (uniq) | UPOS | Avg sent len | Min | Max |
|------|-----------|---------------|---------------|------------|-----|-------|--------------|---------------|------|--------------|-----|-----|
| pro_corag-ud-dev.conllu | 118 | 4,405 | 4,279 | 4,531 | 126 | 0 | 1,261 | 0 | 14 | 37.3 | 4 | 130 |
| pro_corag-ud-test.conllu | 276 | 10,208 | 9,920 | 10,496 | 288 | 0 | 2,454 | 0 | 14 | 37.0 | 4 | 229 |
| pro_corag-ud-train.conllu | 1,092 | 37,926 | 36,829 | 39,023 | 1,097 | 0 | 5,621 | 0 | 14 | 34.7 | 3 | 332 |
| Total | 1,486 | 52,539 | 51,028 | 54,050 | 1,511 | 0 | — | — | — | 35.4 | — | — |

Please note that CorAG treebank is still under development. A campain of revision and morphological annotation is underway and new material is being added to the collection. The structure of the treebank is therefore likely to change in subsequent releases. Please do not hesitate to contact us if you have any questions, suggestions or comments.

# Annotation

The texts were digitized, segmented and subsequently automatically annotated with [HOPS](https://github.com/hopsparser/hopsparser) and [BertForDeprel](https://github.com/kirianguiller/BertForDeprel) parsers using bootstrapping methodology ([Peng et al 2022](https://hal.science/hal-03846834/document)) on [ArboratorGrew](https://arborator.grew.fr/#/) software.

The texts are annotated in PoS and syntactic functions (Universal Dependencies), following, wherever possible, the guidelines for Modern Occitan ([Miletić et al 2020](https://hal.science/hal-04925754v1)).

In addition, for the 2.18 release, verbs and auxiliaries have been annotated in verb forms (VerbForm): Inf (infinitive), Fin (conjugated) and Part (participle). Congujated forms are annotated in Person (1,2,3) and Number (Sing, Plur). Annotation in Mood and Tense is ongoing. Participles are annotated in Tense (Past, Pres, Fut), Gender (Masc, Fem) and Number (Sing, Plur). The annotation in features follows the form of the the token (i.e., forms with no agreement in Gender or Number were annotated as masculine singular). 

Please note that participles without dependents are annotated as adjectives but are also provided with morphological features of participles (VerbForm, Tense, Gender, Number).

Pronouns are annotated in type (PronType: Prs, Dem, Ind, Rel). Reflexive pronouns are annotated as Prs with an additional Poss=Yes feature. Possessive pronouns have the feature Poss=Yes.

Personal pronouns are annotated in Person (1,2,3) and, wherever possible, Number (Sing, Plur), Gender (Masc, Fem, Neut). Neut is used for the pronoun "o".

Demonstrative pronouns are annotated in Number (Sing, Plur) and Gender (Masc, Fem, Neut). Neut is used for pronouns ço (so), ac (ag) and aquet. 

Indefinite pronouns are annotated, wherever possible, in Number (Sing, Plur) and Gender (Masc, Fem).

Relative pronouns have no further morphological annotation at present.

Tokens with negative polarity (that belong to ADJ, ADP, ADV, CCONJ, DET and PRON categories) have Polarity=Neg feature.

# Acknowledgments
The corpus is part of Professor Pierre Larrivée's (University of Caen) [Senior membership project](https://www.iufrance.fr/les-membres-de-liuf/membre/2346-pierre-larrivee.html) with the Institut Universitaire de France.

Manual annotation was performed by [Barbara Francioni](https://cv.hal.science/barbara-francioni) with the help from [Natasha Romanova](https://cv.hal.science/natasha-romanova). Technical support by [Rayan Ziane](https://cv.hal.science/rayan-ziane) and Khensa Daoudi. Digitization by Christelle Violette. Project coordination by Natasha Romanova.

We thank Professor Martin Glessgen and his team at the University of Zurich (authors of the online resource [Documents linguistiques galloromans](https://gallrom.linguistik.uzh.ch/#/) for provinding us with their editions of the thirteenth-century texts included in the corpus.

The version of the treebank from November 2025 can also be consulted and queried via the CRISCO Lab (University of Caen) [TXM portal](https://txm-crisco.huma-num.fr/txm/) where 1240-1314_Deux and 1460_Bearn are also available consultation as a digital edition (Larrivée P. & Francioni B. (ed.) 2026. CorAG Corpus, v. 1.2 (EA 4255). Caen: CRISCO).


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
