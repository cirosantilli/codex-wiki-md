<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The minimizer in the quadratic expression from part (b) is

$$
u_{t-1}^*
=-\frac{P_t}{1+P_t}\widehat x_{t-1}.
$$

Relabelling the time index,

$$
\boxed{u_t^*=-K_t\widehat x_t,\qquad
K_t=\frac{P_{t+1}}{1+P_{t+1}}
=\frac1{T-t+1}.}
$$

If $\operatorname{Var}(x_0)$ or the observation-noise variances change, the [Kalman filter](../../../../../../kalman-filter.md) gains and the sequence $V_t$ change. The control gain $K_t$ does **not** change, because the state dynamics and quadratic cost are unchanged. This is the [separation principle](../../../../../../separation-principle.md): estimation uncertainty changes the additive constants $d_t$, while the optimal linear feedback gain is the full-information gain.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
