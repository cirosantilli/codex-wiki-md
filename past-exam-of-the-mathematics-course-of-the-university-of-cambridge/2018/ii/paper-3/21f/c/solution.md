<h1 id="21f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every finite scalar sequence $a=(a_n)$ with $|a_n|\leq1$, define a bounded linear functional on the [continuous dual space](../../../../../../continuous-dual-space-split.md) $X^*$ by

$$
T_a(f)=\sum_na_nf(x_n).
$$

For each fixed $f\in X^*$, the hypothesis gives

$$
\sup_a|T_a(f)|
=\sum_{n=1}^{\infty}|f(x_n)|<\infty,
$$

where the supremum is over all finite choices and the phases $a_n$ may be chosen to align the complex numbers $f(x_n)$.

The dual $X^*$ is a [Banach space](../../../../../../banach-space-split.md) even when $X$ is incomplete. The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) therefore gives a constant $C$ such that

$$
\sup_a\lVert T_a\rVert\leq C.
$$

For each $N$, choose $a_n$ for $n\leq N$ so that $a_nf(x_n)=|f(x_n)|$. Then

$$
\sum_{n=1}^N|f(x_n)|
=|T_a(f)|
\leq C\lVert f\rVert.
$$

Letting $N\to\infty$ proves

$$
\boxed{\sum_{n=1}^{\infty}|f(x_n)|\leq C\lVert f\rVert
\quad\text{for every }f\in X^*.}
$$

This is the [uniform bound from pointwise absolute summability of dual evaluations](../../../../../../uniform-bound-from-pointwise-absolute-summability-of-dual-evaluations.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21F](../../21f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
