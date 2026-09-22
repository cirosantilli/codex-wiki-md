<h1 id="28l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Q=F^{-1}$ be the [quantile function](../../../../../../quantile-function.md). For $p\in(0,1)$,

$$
Q(p)\leq t\quad\Longleftrightarrow\quad p\leq F(t).
$$

The reverse implication is immediate from the infimum defining $Q$. For the forward implication, if $Q(p)<t$ there is a point $s\leq t$ with $F(s)\geq p$. If $Q(p)=t$, choose $s_m<t+1/m$ with $F(s_m)\geq p$; monotonicity and right continuity give

$$
F(t)=\lim_{m\to\infty}F(t+1/m)\geq p.
$$

The endpoint values $p=0,1$ have zero probability under a continuous uniform variable.

Consequently

$$
\mathbb P(Q(U)\leq t)
=\mathbb P(U\leq F(t))
=F(t).
$$

Thus the [inverse transform sampling](../../../../../../inverse-transform-sampling.md) identity is

$$
\boxed{F^{-1}(U)\sim F}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28L](../../28l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
