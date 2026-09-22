<h1 id="17d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the test equation $y'=\lambda y$, write one numerical step as

$$
y_{n+1}=R(h\lambda)y_n.
$$

The [linear stability domain](../../../../../../linear-stability-domain.md) is

$$
\mathcal S=\{z\in\mathbb C:|R(z)|\leq1\}.
$$

A method is A-stable when $\{z:\Re z\leq0\}\subseteq\mathcal S$.

Forward Euler has $R(z)=1+z$, so

$$
\boxed{\mathcal S_{\rm FE}=\{z:|1+z|\leq1\}}.
$$

This disk does not contain the whole left half-plane, so forward Euler is not A-stable. Backward Euler has $R(z)=(1-z)^{-1}$, so

$$
\boxed{\mathcal S_{\rm BE}=\{z:|1-z|\geq1\}}.
$$

It contains the left half-plane, and backward Euler is A-stable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17D](../../17d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
