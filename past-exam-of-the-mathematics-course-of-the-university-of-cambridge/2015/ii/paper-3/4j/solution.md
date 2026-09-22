<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

The command fits the [simple linear regression](../../../../../simple-linear-regression.md)

$$
Y_i=\beta_0+\beta_1t_i+\varepsilon_i,\qquad \varepsilon_i\ \hbox{independent }N(0,\sigma^2),
$$

using [ordinary least squares](../../../../../ordinary-least-squares.md). The fitted conditional mean is a straight line in time. The [regression residuals](../../../../../regression-residual.md) are mainly positive at the beginning and end and negative in the middle, so the mean function needs curvature.

A direct improvement is [polynomial regression](../../../../../polynomial-regression.md) of degree two:
```
fit2 <- lm(Counts ~ Time + I(Time^2), data = geiger)
anova(fit1, fit2)
```
The nested-model [F-test](../../../../../f-test.md) tests $H_0:\beta_2=0$ against a nonzero quadratic coefficient. If $N$ measurements were used, its statistic is

$$
\boxed{F=\frac{\operatorname{RSS}_1-\operatorname{RSS}_2}{\operatorname{RSS}_2/(N-3)}\sim F_{1,N-3}\quad\hbox{under }H_0.}
$$

A small reported $p$-value supports the quadratic term. The new [regression residuals](../../../../../regression-residual.md) should then be checked for remaining systematic structure, changing variance and temporal dependence, because the [F-test](../../../../../f-test.md) assumes independent errors of common variance. Radioactive decay also motivates an exponential mean, but the displayed curvature already justifies this simple nested comparison.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
