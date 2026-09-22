<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Include an intercept $w_0$ and let $\mathbf z$ be the chosen numerical feature vector. [Logistic regression](../../../../../logistic-regression.md) uses

$$
\boxed{h(\mathbf z;\mathbf w)=\sigma(w_0+\mathbf w^{\mathsf T}\mathbf z),
\qquad\sigma(u)=\frac1{1+e^{-u}}.}
$$

The [logistic function](../../../../../logistic-function.md) maps every real score into $(0,1)$, allowing a [Bernoulli distribution](../../../../../bernoulli-distribution.md) model for the label. Equivalently, the [log odds](../../../../../log-odds.md) are linear in the features:

$$
\log\frac h{1-h}=w_0+\mathbf w^{\mathsf T}\mathbf z.
$$

This gives a smooth differentiable [probability](../../../../../probability.md) model with a linear decision boundary at any fixed [probability](../../../../../probability.md) threshold. The sigmoid output is a fitted conditional [probability](../../../../../probability.md), not a categorical prediction until a threshold is chosen.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
