<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a continuous path $m$ of [finite variation](../../../../../../total-variation-of-a-function.md) on $[0,t]$, every partition satisfies

$$
\sum_j(m_{t_{j+1}}-m_{t_j})^2\leq\max_j|m_{t_{j+1}}-m_{t_j}|\operatorname{Var}_{[0,t]}(m).
$$

Uniform continuity makes the right side tend to zero as the mesh tends to zero. The [quadratic variation](../../../../../../quadratic-variation.md) of the given [continuous local martingale](../../../../../../continuous-local-martingale.md) $M$ is therefore identically zero.

Stop $M$ when its magnitude first reaches an integer $n$, so the stopped process is a bounded, square-integrable [martingale](../../../../../../martingale-split.md). The square identity, or the [Itô isometry](../../../../../../ito-isometry.md), gives $\mathbb E M_{t\wedge\tau_n}^2=\mathbb E[M]_{t\wedge\tau_n}=0$. Hence it is zero at each rational time almost surely, and continuity extends this simultaneously to all times. Let $n$ tend to infinity. This proves

$$
\boxed{M_t=0\text{ for every }t\geq0\text{ on one event of probability one}.}
$$

This is the [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md) principle with initial value zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
