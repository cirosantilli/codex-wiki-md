# Primary clustering

↑ **Parent:** [Linear probing cluster](linear-probing-cluster.md)

In an insertion-only table, an absent [hash table key](hash-table-key.md) starting anywhere inside a [linear probing cluster](linear-probing-cluster.md) reaches its far end. Filling a one-slot gap can merge two runs, joining [hash table keys](hash-table-key.md) with different initial [array indices](array-index.md) into one long search route. The insertion of $10$ above exhibits this effect without a [hash collision](hash-collision.md) with $0$ at their initial slots.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; Lecture 10: Hashing III: Open Addressing, pp. 3–4, Linear Probing and Figure 4: Primary Clustering](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-10-hashing-iii-open-addressing.md)

## ↑ Ancestors (7)

1. [Linear probing cluster](linear-probing-cluster.md)
2. [Linear probing](linear-probing.md)
3. [Open addressing](open-addressing.md)
4. [Hash table](hash-table.md)
5. [Data structure](data-structure-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)
