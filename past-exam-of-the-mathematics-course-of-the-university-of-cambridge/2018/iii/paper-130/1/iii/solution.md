<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $N$ be a word length supplied by the [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) for [alphabet](../../../../../../alphabet.md) $[m]$ and two colors. For $n\geq2N$, embed $[m]^N$ into $[m]^n$ by the [coordinate duplication for combinatorial lines](../../../../../../coordinate-duplication-for-combinatorial-lines.md) map

$$
(x_1,\ldots,x_N)\longmapsto(x_1,x_1,x_2,x_2,\ldots,x_N,x_N,1,\ldots,1).
$$

Pull back any two-color [finite coloring](../../../../../../finite-coloring.md) to this word space. The [Hales-Jewett theorem](../../../../../../hales-jewett-theorem.md) gives a [monochromatic](../../../../../../monochromatic-set.md) [combinatorial line](../../../../../../combinatorial-line.md) with nonempty active set $S$. Its image is a [combinatorial line](../../../../../../combinatorial-line.md) whose active set is

$$
\bigcup_{j\in S}\{2j-1,2j\},
$$

and hence has size $2|S|$, a positive even integer. Therefore

$$
\boxed{\{A\subseteq[n]:|A|\text{ is even}\}\text{ is adequate for all }n\geq2N.}
$$

The empty set's presence in the family causes no difficulty: the line just constructed has at least two active coordinates.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
