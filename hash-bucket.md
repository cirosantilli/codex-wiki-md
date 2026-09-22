# Hash bucket

↑ **Parent:** [Hash table](hash-table.md)

The collection of records assigned to one bucket index by a [hash function](hash-function.md). In [separate chaining](separate-chaining.md), an [array](array-data-structure.md) slot refers to this collection, which may be empty.

For $m>0$ [hash buckets](hash-bucket.md), number them $0,\ldots,m-1$ and write $\ell_j$ for the number of records in [hash bucket](hash-bucket.md) $j$. Each record belongs to exactly one [hash bucket](hash-bucket.md), so

$$
\sum_{j=0}^{m-1}\ell_j=n,\qquad \frac1m\sum_{j=0}^{m-1}\ell_j=\frac nm=\alpha.
$$

An empty [hash bucket](hash-bucket.md) contributes zero to this sum but still contributes one to the denominator $m$. The [hash table load factor](load-factor-of-a-hash-table.md) therefore measures records per allocated [hash bucket](hash-bucket.md), not records per nonempty [hash bucket](hash-bucket.md). A [hash bucket](hash-bucket.md) is a destination selected by the bucket-index [hash function](hash-function.md); with [separate chaining](separate-chaining.md), its records need not occupy consecutive positions in [computer memory](computer-memory.md).

For the twelve-record concentrated placement in [load factor of a hash table](load-factor-of-a-hash-table.md), one [hash bucket](hash-bucket.md) contains twelve records and seven [hash buckets](hash-bucket.md) are empty. Averaging only over nonempty [hash buckets](hash-bucket.md) gives $12$, whereas the [hash table load factor](load-factor-of-a-hash-table.md) is $12/8=1.5$. This difference matters when deciding how much [array](array-data-structure.md) capacity to allocate. For $n>0$, the largest [hash bucket](hash-bucket.md) satisfies $\lceil n/m\rceil\leq\max_j\ell_j\leq n$; the lower bound follows because at least one entry cannot be below the [arithmetic mean](arithmetic-mean.md). Neither inequality says that an actual [hash function](hash-function.md) achieves a balanced placement.

## ↑ Ancestors (4)

1. [Hash table](hash-table.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Hash bucket](hash-bucket.md)
- [Hash table](hash-table.md)
- [Hash table resizing](hash-table-resizing.md)
- [Key equality](key-equality.md)
- [Load factor of a hash table](load-factor-of-a-hash-table.md)
- [Separate chaining](separate-chaining.md)
