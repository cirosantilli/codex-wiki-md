<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The topology needed here is the [weak-star topology](../../../../../../weak-star-topology.md) $\sigma(E^*,E)$, meaning pointwise convergence on $E$. With the literal [weak topology](../../../../../../weak-topology-split.md) $\sigma(E^*,E^{**})$, the claimed [compactness](../../../../../../compact-space.md) is false. For example, $E=c_0$ is separable and $E^*=\ell^1$. Its unit [vectors](../../../../../../vector.md) $e_n$ have no weak cluster point: every coordinate functional forces a cluster point to have all coordinates zero, while the bounded functional $x\mapsto\sum_jx_j$ has value one throughout. Thus the dual [unit ball](../../../../../../unit-ball.md) is not [weakly compact](../../../../../../weakly-compact-set.md). We prove the intended weak-star assertion in full.

Choose a countable dense set $(x_k)$ in the [unit ball](../../../../../../unit-ball.md) of $E$. On $E_1^*$ define

$$
\boxed{d(\phi,\psi)=\sum_{k\geq1}2^{-k}|\phi(x_k)-\psi(x_k)|.}
$$

Each term is at most $2\cdot2^{-k}$, so the series converges. The [triangle inequality](../../../../../../triangle-inequality.md) is immediate, and $d=0$ forces equality on the dense set and hence on all of $E$. It is therefore a metric. Convergence in this metric is equivalent to convergence on every $x_k$: one direction follows from any individual term, and the other by bounding the series tail uniformly. Because $\|\phi\|,\|\psi\|\leq1$, approximation of any unit [vector](../../../../../../vector.md) by $x_k$ then gives convergence on all of $E$. The same finite-tail and approximation argument for neighborhoods proves equality with the [weak-star topology](../../../../../../weak-star-topology.md), not just agreement of its convergent sequences.

Given a sequence $(\phi_n)$ in this ball, diagonal selection gives a subsequence converging at every $x_k$, since each coordinate lies in a compact disk. Uniform [norm](../../../../../../norm.md) bounds then make it pointwise Cauchy at every $x\in E$. Define $\phi(x)$ as the limit. [Linearity](../../../../../../linearity.md) passes to the limit, and $|\phi(x)|\leq\|x\|$, so $\phi\in E_1^*$. The subsequence converges to it in the metric. Thus this [metric space](../../../../../../metric-space.md) is sequentially compact, hence compact, proving

$$
\boxed{E_1^*\text{ is compact and metrizable in }\sigma(E^*,E).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
