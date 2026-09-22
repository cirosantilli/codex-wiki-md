<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [simple predictable process](../../../../../../simple-predictable-process.md) has the form $H_s=\sum_{j=0}^{m-1}h_j\mathbf1_{(t_j,t_{j+1}]}(s)$, where $0=t_0<\cdots<t_m<\infty$ are deterministic and $h_j$ is bounded and $\mathcal F_{t_j}$-measurable. A possible $\mathcal F_0$-measurable value at zero is irrelevant to this [Itô integral](../../../../../../ito-integral.md). Define

$$
\boxed{(H\mathbin\cdot M)_t=\sum_{j=0}^{m-1}h_j\bigl(M_{t\wedge t_{j+1}}-M_{t\wedge t_j}\bigr).}
$$

Each coefficient is known before the corresponding increment. The [conditional expectation](../../../../../../conditional-expectation.md) of each subsequent increment is zero, so the result is a continuous [martingale](../../../../../../martingale-split.md) starting at zero. It is an [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md) because it is a finite sum of bounded coefficients times stopped increments of an [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md). This definition is independent of the chosen subdivision: splitting an interval simply splits its increment into a telescoping sum. General admissible [predictable processes](../../../../../../predictable-process.md) are then integrated by completion using the [Itô isometry](../../../../../../ito-isometry.md); unbounded step coefficients are allowed when the weighted $L^2$ condition in the [quadratic-variation measure](../../../../../../quadratic-variation-measure.md) in the next part holds.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
