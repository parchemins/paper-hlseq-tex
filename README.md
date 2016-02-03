# Concurrency Effects Over Variable-size Identifiers in Distributed Collaborative Editing

<i>Keywords: Distributed Documents; Document Authoring Tools and Systems;
Distributed Collaborative Editing; Real-time Editing; Conflict-free Replicated
Data Types</i>

<i>Authors: Brice Nédelec, Pascal Molli, Achour Mostefaoui, Emmanuel
Desmontils</i>

Distributed collaborative editors such as Google Docs or Etherpad allow to
distribute the work across time, space and organizations. In this paper, we
focus on distributed collaborative editors based on the Conflict-free
Replicated Data Type approach (CRDT). CRDTs encompass a set of well-known data
types (sets, graphs, sequences, etc.). CRDTs for sequences model a document as
a set of elements (character, line, paragraph, etc.) with unique identifiers,
providing two commutative update operations: insert and delete. The identifiers
of elements can be either of fixed-size or variable-size. Recently, a strategy
for assigning variable-size identifiers called LSEQ has been proposed for CRDTs
for sequences. LSEQ lowers the space complexity of variable-size identifiers
CRDTs from linear to sub-linear. While experiments show that it works locally,
it fails to provide this bound with multiple users and latency. In this paper,
we propose h-LSEQ, an improvement of LSEQ that preserves its space complexity
among all collaborators, regardless of the latency. Ultimately, this
improvement allows to safely build distributed collaborative editors based on
CRDTs. We validate our approach with simulations involving latency and multiple
users.

## Available at

<ul>
  <li> [HAL](https://hal.archives-ouvertes.fr/hal-00921655)
</ul>

## BibTeX

```
@inproceedings{nedelec:hal-00921655,
  TITLE = {{Concurrency Effects Over Variable-size Identifiers in Distributed
            Collaborative Editing}},
  AUTHOR = {N{\'e}delec, Brice and Molli, Pascal and Mostefaoui, Achour and
            Desmontils, Emmanuel},
  URL = {https://hal.archives-ouvertes.fr/hal-00921655},
  NOTE = {7 pages},
  BOOKTITLE = {{Document Changes: Modeling, Detection, Storage and
                Visualization}},
  ADDRESS = {Florence, Italy},
  SERIES = {CEUR Workshop Proceedings},
  VOLUME = {1008},
  PAGES = {0--7},
  YEAR = {2013},
  MONTH = Sep,
  KEYWORDS = {Distributed Documents ; Document Authoring Tools and Systems ;
              Distributed Collaborative Editing ; Real-time Editing ;
              Conflict-free Replicated Data Types}
}
```

## Acknowledgments

This work was partially funded by the French ANR project ConcoRDanT
([ANR-10-BLAN-0208](http://www.agence-nationale-recherche.fr/?Projet=ANR-10-BLAN-0208)).
