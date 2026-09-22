<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conditioned on exactly $k$ heads, every $k$-element set of head positions is equally likely. There are $\binom nk$ such sets. A run containing all $k$ heads can begin at any of the positions

$$
1,2,\ldots,n-k+1,
$$

and each beginning determines one admissible set. Thus, for $k\geq1$,

$$
\boxed{
\mathbb P(\text{the }k\text{ heads are consecutive}\mid
\text{exactly }k\text{ heads})
=\frac{n-k+1}{\binom nk}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
