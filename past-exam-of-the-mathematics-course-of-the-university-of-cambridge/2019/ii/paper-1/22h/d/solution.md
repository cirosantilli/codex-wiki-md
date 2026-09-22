<h1 id="22h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume for contradiction that $X$ is infinite-dimensional. Starting with $M_0=\{0\}$, apply [Riesz lemma](../../../../../../riesz-s-lemma.md) recursively to the proper closed finite-dimensional subspaces

$$
M_{n-1}=\operatorname{span}\{x_1,\ldots,x_{n-1}\}
$$

to choose unit vectors $x_n$ satisfying

$$
\operatorname{dist}(x_n,M_{n-1})>\frac12.
$$

For $m<n$, the vector $x_m$ belongs to $M_{n-1}$, and therefore

$$
\lVert x_n-x_m\rVert>\frac12.
$$

Thus $(x_n)$ lies in the closed unit ball but has no [Cauchy subsequence](../../../../../../cauchy-subsequence.md), hence no convergent subsequence. A compact metric space is [sequentially compact](../../../../../../sequentially-compact-space.md), contradicting compactness of the unit ball. Therefore $X$ is finite-dimensional, proving that a [compact unit ball characterizes finite-dimensional normed spaces](../../../../../../compact-unit-ball-characterizes-finite-dimensional-normed-spaces.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [22H](../../22h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
