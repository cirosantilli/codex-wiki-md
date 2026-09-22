<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a bounded measurable $f$, the dual estimate for [total variation distance](../../../../../../total-variation-distance.md) gives

$$
\left|\int f\,d\mu_n-\int f\,d\mu\right|
\leq2\lVert f\rVert_\infty
\sup_A|\mu_n(A)-\mu(A)|.
$$

The right-hand side tends to zero, so in particular the integrals converge for every bounded continuous $f$. Thus [weak convergence of random variables](../../../../../../convergence-in-distribution.md) follows.

The converse fails. On $\mathbb R$, let $\mu_n=\delta_{1/n}$ and $\mu=\delta_0$. Continuity gives $f(1/n)\to f(0)$, so $\mu_n$ converges weakly to $\mu$. However, for $A=\{0\}$,

$$
|\mu_n(A)-\mu(A)|=1
$$

for every $n$, so there is no convergence in [total variation distance](../../../../../../total-variation-distance.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
