Papers 2013
===========

Contains all papers in branches. A branch suffixed by a "s" letter refers to
the submission version of the paper. The master branch tracks current work.

DChanges2013
------------

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

DocEng2013
----------

Distributed collaborative editing systems allow users to work distributed in
time, space and across organizations. Trending distributed collaborative
editors such as Google Docs, Etherpad or Git have grown in popularity over the
years. A new kind of distributed editors based on a family of distributed data
structure replicated on several sites called Conflict-free Replicated Data Type
(CRDT for short) appeared recently. This paper considers a CRDT that represents
a distributed sequence of basic elements that can be lines, words or characters
(sequence CRDT). The possible operations on this sequence are the insertion and
the deletion of elements. Compared to the state of the art, this approach is
more decentralized and better scales in terms of the number of
participants. However, its space complexity is linear with respect to the total
number of inserts and the insertion points in the document. This makes the
overall performance of such editors dependent on the editing behaviour of
users. This paper proposes and models LSEQ, an adaptive allocation strategy
for a sequence CRDT. LSEQ achieves in the average a sub-linear
spatial-complexity whatever is the editing behaviour. A series of experiments
validates LSEQ showing that it outperforms existing approaches.
