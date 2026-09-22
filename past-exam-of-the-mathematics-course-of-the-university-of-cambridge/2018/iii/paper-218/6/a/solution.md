<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the residual-versus-fitted plot, compute [fitted values](../../../../../../fitted-values.md) $\widehat y_i=\widehat\beta_0+\widehat\beta_1x_{i1}+\widehat\beta_2x_{i2}$ and [regression residuals](../../../../../../regression-residual.md) $e_i=y_i-\widehat y_i$; the plotted point is $(\widehat y_i,e_i)$.

For the normal [Q-Q plot](../../../../../../q-q-plot.md), let $H=X(X^TX)^{-1}X^T$ be the [hat matrix](../../../../../../hat-matrix.md) for the full three-column [design matrix](../../../../../../design-matrix.md) and let $s^2=\operatorname{RSS}/(n-3)$. Form the [standardized regression residuals](../../../../../../standardized-regression-residual.md)

$$
r_i=\frac{e_i}{s\sqrt{1-h_{ii}}}
$$

and order them as $r_{(1)}\leq\cdots\leq r_{(n)}$. R plots $r_{(j)}$ against $\Phi^{-1}(p_j)$, where $p_j$ are its plotting positions. For $n>10$, $p_j=(j-1/2)/n$; $\Phi$ is the [standard normal distribution](../../../../../../standard-normal-distribution.md) function. This standardization is specified in [R's diagnostic-plot documentation](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/plot.lm.html).

The original PDF shows a residual cloud around zero without compelling systematic curvature or a clear funnel, and a Q-Q pattern approximately following the reference line. Observations 81 and 83 are conspicuous positive tail points, with a smaller lower-tail departure. **The plots show no decisive violation of linearity, constant variance or normality, but the extreme residuals merit inspection.** They do not test independence across observations and cannot establish that all model assumptions hold.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
