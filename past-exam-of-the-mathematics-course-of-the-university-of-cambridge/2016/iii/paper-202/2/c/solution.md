<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The **[Novikov condition](../../../../../../novikov-s-condition.md) holds on every horizon**, since

$$
\mathbb E\exp\{\tfrac12[M]_T\}\leq e^{C/2}<\infty.
$$

Therefore $Z=\mathcal E(M)$ is a true [martingale](../../../../../../martingale-split.md) and the [Girsanov theorem](../../../../../../girsanov-theorem.md) applies through each finite $T$.

The deterministic bound also gives a genuine infinite-horizon density. For any $p>1$, the [stochastic exponential](../../../../../../doleans-dade-exponential.md) identity is

$$
Z_t^p=\mathcal E(pM)_t\exp\{\tfrac12p(p-1)[M]_t\}.
$$

A nonnegative [local martingale](../../../../../../local-martingale.md) is a [supermartingale](../../../../../../supermartingale.md), so

$$
\boxed{\sup_t\mathbb E Z_t^p\leq\exp\{\tfrac12p(p-1)C\}.}
$$

This $L^p$ bound gives [uniform integrability](../../../../../../uniform-integrability.md). Also $M$ is a [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md), since localization and the [Itô isometry](../../../../../../ito-isometry.md) give $\mathbb E M_t^2=\mathbb E[M]_t\leq C$. The [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) gives a finite limit $M_\infty$; hence $Z_\infty=\exp(M_\infty-[M]_\infty/2)>0$ and $\mathbb E Z_\infty=1$. Weighting by $Z_\infty$ defines an equivalent [probability measure](../../../../../../probability-measure.md) on $\mathcal F_\infty$. This is the [bounded-bracket criterion for a stochastic exponential](../../../../../../bounded-bracket-criterion-for-a-stochastic-exponential.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
