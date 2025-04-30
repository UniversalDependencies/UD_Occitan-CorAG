# Summary
UD_Occitan-CorAG (Corpus de l'Ancien Gascon) is a corpus of medieval legal texts in Gascon, a variety of Old Occitan. The texts were digitized from printed editions and subsequently manually annotated in Universal Dependencies (PoS and functions).

# Introduction

The collection currently contains two texts:

\* _Coutumes et Privilèges de l’Entre-Deux-Mers_, 1214-1342 (Lépicier 1861): 344 sentences; 11,975 tokens

\* _Les Fors Anciens de Béarn_ 1460 (Ourliac & Gilles 1990): 750 sentences ; 26,704 tokens

The texts were digitized, segmented and subsequently automatically annotated with [HOPS](https://github.com/hopsparser/hopsparser) and [BertForDeprel](https://github.com/kirianguiller/BertForDeprel)) parsers using bootstrapping methodology (Peng et al 2022) on [ArboratorGrew](https://arborator.grew.fr/#/) software.

| Set               | Sentences| Tokens    |
| :---------------- | :------: | ----:     |
| Train             |   657    |   23,807  |
| Dev               |   152    |   4,580   |
| Test              |   285    |   10,292  |
| **Total**         | **1,094**| **38,676**|


# Acknowledgments
The corpus is part of Professor Pierre Larrivée's (University of Caen) [Senior membership project](https://www.iufrance.fr/les-membres-de-liuf/membre/2346-pierre-larrivee.html) with the Institut Universitaire de France. Manual annotation was performed by Barbara Francioni. Technical support by Rayan Ziane and Khensa Daoudi. Digitization by Christelle Violette. Project coordination by Natasha Romanova.

## References

* Forthcoming


# Changelog

* 2025-05-15 v2.16
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.16
License: CC BY-SA 4.0
Includes text: yes
Genre: legal
Lemmas: not available
UPOS: manual native
XPOS: not available
Features: not available
Relations: manual native
Contributors: Barbara Francioni; Romanova, Natalia; Ziane, Rayan; Daoudi, Khensa; Larrivée, Pierre
Contributing: here
Contact: natalia.romanova@unicaen.fr
===============================================================================
</pre>
