<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Substitute the [linear regression model](../../../../../../../linear-regression-model.md) into the estimators and use the centring and [orthogonality](../../../../../../../orthogonal-vectors.md) conditions:

$$
\widehat\beta_0=\beta_0+\frac1n\sum_i\epsilon_i,\qquad
\widehat\beta_1=\beta_1+\frac{\sum_i x_i\epsilon_i}{S_{xx}}.
$$

A linear combination of [independent](../../../../../../../independent-random-variables.md) [normal random variables](../../../../../../../gaussian-random-variable.md) is normal. Their [means](../../../../../../../expected-value-split.md) are $\beta_0$ and $\beta_1$, while [variance additivity for independent random variables](../../../../../../../variance-additivity-for-independent-random-variables.md) gives

$$
\operatorname{Var}(\widehat\beta_0)=\frac{n\sigma^2}{n^2}=\frac{\sigma^2}{n},\qquad
\operatorname{Var}(\widehat\beta_1)=\frac{\sigma^2\sum_i x_i^2}{S_{xx}^2}=\frac{\sigma^2}{S_{xx}}.
$$

Consequently

$$
\boxed{\widehat\beta_0\sim N(\beta_0,\sigma^2/n),\qquad
\widehat\beta_1\sim N(\beta_1,\sigma^2/S_{xx}).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
