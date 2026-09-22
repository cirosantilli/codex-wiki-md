# Linear probing cluster

↑ **Parent:** [Linear probing](linear-probing.md)

A maximal consecutive run of occupied or deleted slots in [linear probing](linear-probing.md), bounded by never-used slots when any exist; adjacency wraps around by [modular arithmetic](modular-arithmetic-split.md). Deleted slots still belong to the search run.[Open Data Structures: An Introduction by Pat Morin; Section 5.2.1, definition of a run using non-nil entries and modular indices](open-data-structures-an-introduction-by-pat-morin/5-2-linearhashtable-linear-probing.md)

In the eight-slot example, [array indices](array-index.md) $0,1,2,3$ form one [linear probing cluster](linear-probing-cluster.md). Inserting absent [hash table key](hash-table-key.md) $10$ starts at $2$, passes the occupied slots $2,3$, and fills $4$. This extends the same [linear probing cluster](linear-probing-cluster.md) despite $10$ having a different initial [array index](array-index.md) from $0,8,16$. A [hash collision](hash-collision.md) at the initial slot is enough to make later slots compete too.

For a worst-case family, insert [integer](integer-split.md) [hash table keys](hash-table-key.md) $0,m,2m,\ldots,(n-1)m$ into an empty capacity-$m$ [array](array-data-structure.md), using the [hash function](hash-function.md) $h_m(k)=k\bmod m$, where $1\leq n<m$. They occupy [array indices](array-index.md) $0,\ldots,n-1$. Lookup of absent $nm$ needs $n+1$ [hash table probes](hash-table-probe.md). Taking $n=\lfloor m/2\rfloor$ gives [hash table load factor](load-factor-of-a-hash-table.md) at most $1/2$ while the number of [hash table probes](hash-table-probe.md) grows with $m$. Thus occupancy alone cannot promise constant lookup work.

Before any rebuilding, bounded lookup, deletion by [hash table key](hash-table-key.md), and insertion with a duplicate check each have worst-case $O(m)$ [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md), assuming constant-cost [hash function](hash-function.md) evaluation, [array](array-data-structure.md) access and [key equality](key-equality.md). The counterexample gives a matching linear worst-case growth in the number of [hash table probes](hash-table-probe.md). [Hash table resizing](hash-table-resizing.md) is additional work; expensive [string](string.md) comparisons or hashing also fall outside these constant-cost assumptions.

**Table of contents**

- [Primary clustering](primary-clustering.md)

## ↑ Ancestors (6)

1. [Linear probing](linear-probing.md)
2. [Open addressing](open-addressing.md)
3. [Hash table](hash-table.md)
4. [Data structure](data-structure-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Linear probing](linear-probing.md)
- [Linear probing cluster](linear-probing-cluster.md)
- [Primary clustering](primary-clustering.md)
- [Tombstone in open addressing](tombstone-in-open-addressing.md)
