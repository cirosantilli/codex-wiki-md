<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $R_i=1$ indicate an observed outcome. Fitting the conditional outcome model to responders requires

$$
\boxed{Y_i\perp R_i\mid x_i,Z_i,}
$$

with a positive observation probability over the relevant predictor support. This is conditional [missing at random](../../../../../../missing-at-random.md) for the predictors used in the regression: after conditioning on them, observation must not further select participants by their unobserved outcome. It gives $f(Y_i\mid x_i,Z_i,R_i=1)=f(Y_i\mid x_i,Z_i)$, the [complete-case regression under conditional missing at random](../../../../../../complete-case-regression-under-conditional-missing-at-random.md) condition. Correct specification of the conditional mean model is also required. [Missing completely at random](../../../../../../missing-completely-at-random.md) is sufficient but stronger; simply assuming missingness depends only on a post-randomization variable excluded from this model would not suffice.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
