<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is [linked file allocation](../../../../../linked-file-allocation.md). A [file header](../../../../../file-header.md) holds the first and last [disk block numbers](../../../../../disk-block-number.md), and the successor field in each block extends the chain. The header therefore does not impose a fixed small maximum number of blocks per file.

To state a numerical bound, suppose a physical block has $B$ bytes, the successor-or-final-count field occupies $h$ bytes, and $N$ distinct data blocks are both addressable and available. A full block then holds $C=B-h$ payload bytes. If the final count can represent every value up to $C$,

$$
\boxed{L\leq NC=N(B-h).}
$$

A smaller [computer file](../../../../../computer-file.md) can use an arbitrary number of full payload blocks followed by a partial block, so allocation need not be contiguous. With a $p$-bit [disk block number](../../../../../disk-block-number.md), $N\leq2^p$, reduced by reserved addresses and blocks consumed by other data and metadata. This gives the address-width bound as well as the actual device-space bound.

There is no positive minimum payload size: an empty [computer file](../../../../../computer-file.md) can be represented by an empty-chain convention or a zero-count terminal block. The question does not specify which representation is used or the relevant field widths, so it does not determine an absolute byte limit or a particular empty-file encoding. Its description presupposes a convention that distinguishes a successor value from a terminal byte count.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
