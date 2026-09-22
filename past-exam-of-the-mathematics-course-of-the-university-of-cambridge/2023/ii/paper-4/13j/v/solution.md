<h1 id="13j/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The fitted [Poisson regression](../../../../../../poisson-regression.md) has

$$
Y_i\mid x_i\sim\operatorname{Pois}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1\log x_i,
$$

so that $\mu_i=e^{\beta_0}x_i^{\beta_1}$. Hypothesis $H_2$ requires both restrictions

$$
\beta_0=0,\qquad \beta_1=1,
$$

as well as the adequacy of the assumed [Poisson distribution](../../../../../../poisson-distribution.md). The displayed interval addresses only the single slope restriction $\beta_1=1$. Even if the separate interval for the intercept also contains zero, separate one-parameter intervals do not implement the relevant [joint hypothesis test](../../../../../../joint-hypothesis-test.md), because the two coefficient estimators can be correlated. One should test $(\beta_0,\beta_1)=(0,1)$ jointly, for example by a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md), and separately assess the Poisson goodness of fit. Thus the slope interval alone cannot decide whether $H_2$ is rejected at the $5\%$ level.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [13J](../../13j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
