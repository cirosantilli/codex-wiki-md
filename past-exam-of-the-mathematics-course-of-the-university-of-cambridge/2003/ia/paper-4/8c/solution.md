<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For each of the $n$ arguments of a [function](../../../../../function-split.md) $X\to X$, there are $n$ choices of image, independently. Thus there are $n^n$ functions. A [binary relation](../../../../../binary-relation.md) is a subset of the $n^2$ ordered pairs in $X\times X$, giving $2^{n^2}$ relations.

Represent a [binary relation](../../../../../binary-relation.md) by its incidence [matrix](../../../../../matrix.md), with row $x$ and column $y$. Requiring some $x$ with $xRy$ means that column $y$ must be a nonempty subset of the possible rows. Each column therefore has $2^n-1$ choices, independently, giving

$$
\boxed{(2^n-1)^n}
$$

relations with no empty column.

To impose no empty row as well, apply the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) within this already column-nonempty family. Let $A_x$ be the family whose row $x$ is empty. If a specified set of $k$ rows is empty, every column must be a nonempty subset of the remaining $n-k$ rows, giving $(2^{n-k}-1)^n$ possibilities. There are $\binom nk$ ways to choose those empty rows. Thus the number with neither an empty row nor an empty column is

$$
\boxed{\sum_{k=0}^n(-1)^k\binom nk(2^{n-k}-1)^n}.
$$

This is the [binary relations with no empty row or column](../../../../../binary-relations-with-no-empty-row-or-column.md) count. It does not require symmetry or transitivity of the relation. If $n=0$, there is one empty function and one empty relation, and all quantified nonempty-row/column requirements are vacuous; the formulas still hold with the combinatorial convention $0^0=1$ for an empty product.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
