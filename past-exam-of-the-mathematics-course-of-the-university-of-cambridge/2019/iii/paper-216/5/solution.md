<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Introduce $Z_{ij}\in\{0,1\}$, where $Z_{ij}=1$ means that the observation came from the structural-zero component. Conditional on the parameters,

$$
\Pr(Z_{ij}=1\mid Y_{ij})=
\begin{cases}
\displaystyle\frac{\pi_j}{\pi_j+(1-\pi_j)e^{-\alpha_i\beta_j}},&Y_{ij}=0,\\
0,&Y_{ij}>0.
\end{cases}
$$

Given $Z$, the nonstructural observations are independent Poisson variables. Using shape-rate parameterization and the stated unit-rate priors, the remaining Gibbs updates are

$$
\alpha_i\mid-\sim\operatorname{Gamma}\left(
1+\sum_j(1-Z_{ij})Y_{ij},
1+\sum_j(1-Z_{ij})\beta_j
\right),
$$



$$
\beta_j\mid-\sim\operatorname{Gamma}\left(
1+\sum_i(1-Z_{ij})Y_{ij},
1+\sum_i(1-Z_{ij})\alpha_i
\right),
$$



$$
\pi_j\mid-\sim\operatorname{Beta}\left(
1+\sum_iZ_{ij},
1+n-\sum_iZ_{ij}
\right).
$$

Alternating these four standard-distribution updates defines the requested [Gibbs sampler](../../../../../gibbs-sampler.md) for the [Zero-inflated Poisson distribution](../../../../../zero-inflated-poisson-distribution.md) posterior.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 216](../../paper-216-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
