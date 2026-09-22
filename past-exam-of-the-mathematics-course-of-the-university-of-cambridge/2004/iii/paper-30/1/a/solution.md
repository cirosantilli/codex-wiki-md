<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $N$ be the zero-starting [continuous local martingale](../../../../../../continuous-local-martingale.md), and let $V_t$ be the total variation of its path on $[0,t]$. Stop when $|N|$ or $V$ reaches $n$, and also at time $n$. The stopped process is bounded, hence a true [square-integrable](../../../../../../square-integrable-function.md) [martingale](../../../../../../martingale-split.md) by the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md), and its total variation is bounded by $n$.

For a deterministic partition $0=t_0<\cdots<t_m=t$, [martingale](../../../../../../martingale-split.md) increments are orthogonal in $L^2$, so

$$
\mathbb E(N_{t\wedge\tau_n}^2)=\sum_j\mathbb E(N_{t_j\wedge\tau_n}-N_{t_{j-1}\wedge\tau_n})^2.
$$

The sum inside the [expectation](../../../../../../expected-value.md) is at most the largest absolute increment times the stopped total variation. As the mesh tends to zero, path continuity makes the largest increment tend to zero. The product is bounded by $2n^2$, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) makes the displayed [expectation](../../../../../../expected-value.md) zero. Thus the stopped process vanishes at every fixed time. Use rational times, continuity and $\tau_n\uparrow\infty$ to conclude

$$
\boxed{N_t=0\text{ for all }t\ge0\text{ outside one null set}.}
$$

This proves that a [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md).

Write a normalized [semimartingale decomposition](../../../../../../semimartingale-decomposition.md) as $X=X_0+N+A$, with both $N_0=A_0=0$, $N$ a [continuous local martingale](../../../../../../continuous-local-martingale.md) and $A$ of [finite variation](../../../../../../total-variation-of-a-function.md). The difference of two such [martingale](../../../../../../martingale-split.md) parts is also the difference of two finite-variation parts, and hence vanishes by the result just proved. The other parts coincide too. **The normalized [continuous semimartingale](../../../../../../continuous-semimartingale.md) decomposition is unique.** Fixing the initial constants is necessary: without normalization a constant can be transferred between the two parts.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
