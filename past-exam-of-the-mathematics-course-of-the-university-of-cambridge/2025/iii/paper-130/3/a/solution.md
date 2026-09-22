<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $c_1,\ldots,c_n$ be the columns of the rational [partition regular matrix](../../../../../../partition-regular-matrix.md) $A$, and clear denominators so that they are integer vectors. We use the [P-adic columns lemma](../../../../../../p-adic-columns-lemma.md). For a large [prime number](../../../../../../prime-number.md) $p$, color each positive integer by a sufficiently long initial block of the unit part of its [P-adic valuation](../../../../../../p-adic-valuation.md), together with its valuation modulo the block length. Partition regularity supplies a monochromatic $x=(x_1,\ldots,x_n)$ with

$$
\sum_{i=1}^n x_i c_i=0.
$$

Group the indices according to the successive $p$-adic orders of the $x_i$. At the lowest order, division by the common power of $p$ and reduction modulo the chosen large power shows

$$
\sum_{i\in B_1}c_i=0.
$$

Comparing the next nonzero blocks of base-$p$ digits shows successively that

$$
\sum_{i\in B_j}c_i\in
\operatorname{span}_{\mathbb Q}\{c_i:i\in B_1\cup\cdots\cup B_{j-1}\}
\qquad(j>1).
$$

For completeness, these congruences may be made exact by taking the digit block longer than every determinant and coordinate formed from the fixed columns: a nonzero such integer cannot be divisible by the resulting power of $p$. There are only finitely many ordered partitions of $[n]$, so passing through arbitrarily long blocks leaves one partition satisfying all the displayed identities. This is precisely the [columns property](../../../../../../columns-property.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
