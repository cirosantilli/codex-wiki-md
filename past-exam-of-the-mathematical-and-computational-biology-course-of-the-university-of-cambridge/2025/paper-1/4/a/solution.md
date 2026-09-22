<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For observation $j$ of bird $i$ in year $t(i,j)$, a [Gaussian linear mixed model](../../../../../gaussian-linear-mixed-model.md) with crossed [random intercepts](../../../../../random-intercept.md) is

$$
Y_{ij}=\beta_0+\beta_1 a_{ij}+u_i+v_{t(i,j)}+\varepsilon_{ij},
\quad
u_i\sim N(0,\tau_b^2),\quad v_t\sim N(0,\tau_y^2),\quad
\varepsilon_{ij}\sim N(0,\sigma^2),
$$

where the $u_i$, $v_t$, and $\varepsilon_{ij}$ are mutually [independent random variables](../../../../../independent-random-variables.md). Here $a_{ij}$ is age, $\beta_0$ is the population intercept at age zero, and $\beta_1$ is the change in conditional [expected value](../../../../../expected-value-split.md) per year of age. The $u_i$ capture persistent between-bird variation, the $v_t$ capture shared annual conditions, and the [regression residuals](../../../../../regression-residual.md) capture remaining observation-level variation. Two observations from the same bird share [covariance](../../../../../covariance.md) $\tau_b^2$; two from the same year share $\tau_y^2$, with both contributions present if both group labels agree. The model also assumes the [random effects](../../../../../random-effect.md) are independent of the age covariate.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
