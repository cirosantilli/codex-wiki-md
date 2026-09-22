<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write

$$
R_i=(x_i-\widehat f(z_i))(y_i-\widehat g(z_i))
=(\varepsilon_i+F_i)(\xi_i+G_i).
$$

Expanding $R_i^2$ gives the leading term $\varepsilon_i^2\xi_i^2$ and terms of the forms treated in parts b and c, together with their versions obtained by interchanging $(\varepsilon,F)$ and $(\xi,G)$. For example, the pure error terms are $\varepsilon_i^2G_i^2$, $\xi_i^2F_i^2$, and $F_i^2G_i^2$, and each cross term is controlled by [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) from these. Hence

$$
\tau_D^2=\frac1n\sum_iR_i^2
=\frac1n\sum_i\varepsilon_i^2\xi_i^2+o_p(1)
\xrightarrow{p}\mathbb E(\varepsilon_1^2\xi_1^2).
$$

Assuming this limit is positive, the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) yields $\tau_D\xrightarrow{p}\{\mathbb E(\varepsilon_1^2\xi_1^2)\}^{1/2}$. Combining this with the assumed [convergence in distribution](../../../../../../convergence-in-distribution.md) of $\sqrt n\tau_N$ and applying the [Slutsky theorem](../../../../../../slutsky-theorem.md) gives

$$
T=\frac{\sqrt n\tau_N}{\tau_D}\xrightarrow{d}N(0,1).
$$

This is the [studentization of the generalized covariance measure statistic](../../../../../../studentization-of-the-generalized-covariance-measure-statistic.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
