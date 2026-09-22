<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Age changes during follow-up, so the [generator matrix](../../../../../../generator-matrix.md) $Q(s)$ changes with time. The [transition matrix](../../../../../../stochastic-matrix.md) must solve $\partial_{t_2}P(t_1,t_2)=P(t_1,t_2)Q(t_2)$, with $P(t_1,t_1)=I$. It is generally not the [matrix exponential](../../../../../../matrix-exponential.md) of one constant matrix; even $\exp(\int Q(s)\,ds)$ is not generally valid because the matrices at different times need not commute.

For example, write the age-dependent onset rate as $\lambda(s)$ and keep progression rate $\nu$ constant. Then

$$
P_{12}(t_1,t_2)=\int_{t_1}^{t_2}\lambda(u)\exp\left(-\int_{t_1}^u\lambda(v)\,dv\right)e^{-\nu(t_2-u)}\,du.
$$

Even when the integrated onset rate is elementary, this remaining integral need not have an elementary closed form. Special cases can have closed forms; time dependence does not by itself prove universal impossibility.

For a tractable [likelihood function](../../../../../../likelihood-function.md), freeze age at its left-endpoint value, or a midpoint value, on each observation interval $[t_j,t_{j+1})$. The genetic [covariate](../../../../../../covariate.md) is already constant. This [piecewise-constant covariate approximation](../../../../../../piecewise-constant-covariate-approximation.md) gives a constant matrix $Q_j$ on each interval and **a product of closed-form interval probabilities**:

$$
\boxed{L=\prod_j\left[e^{Q_j(t_{j+1}-t_j)}\right]_{x_jx_{j+1}}.}
$$

Here $x_j$ is the observed state at $t_j$, and the [likelihood function](../../../../../../likelihood-function.md) is conditional on the initial state. The approximation improves when intervals are short relative to the variation in the age effect.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
