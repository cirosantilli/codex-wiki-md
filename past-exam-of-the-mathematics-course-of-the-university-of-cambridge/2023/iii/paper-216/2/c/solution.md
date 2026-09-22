<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $w(\theta)=\pi(\theta)/\mu(\theta)$ be the [importance weight](../../../../../../importance-weight.md). The two normalized densities give

$$
\log w(\theta)
=-\lambda_2\{Z(\theta)-F(\theta)\}
-\widetilde Z(\lambda)+\widetilde F(\lambda).
$$

Since $|F-Z|<C$, there is a finite constant $M$ such that $w(\theta)\leq M$ everywhere. The [Independence Metropolis–Hastings algorithm](../../../../../../independence-metropolis-hastings-algorithm.md) has an accepted transition density satisfying

$$
\mu(y)\min\left\{1,\frac{w(y)}{w(x)}\right\}
\geq\frac1M\mu(y)w(y)
=\frac1M\pi(y).
$$

Consequently the whole state space is a [small set](../../../../../../small-set.md), with the one-step [minorization condition](../../../../../../minorization-condition.md) $K(x,\mathord\cdot)\geq M^{-1}\pi(\mathord\cdot)$. Iterating this [Doeblin condition](../../../../../../doeblin-s-condition.md) gives uniform geometric convergence in [total variation distance](../../../../../../total-variation-distance.md), so the chain is geometrically ergodic.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
