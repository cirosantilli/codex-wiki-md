<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The common [normal distribution](../../../../../../normal-distribution.md) for the child-specific [random intercepts](../../../../../../random-intercept.md) produces [partial pooling](../../../../../../partial-pooling.md). Children with little information borrow strength from the common population, while well-observed children retain more of their individual estimate. For fixed slopes and hyperparameters, let $\overline r_i$ average the three responses after subtracting their slope terms. Multiplying the normal [likelihood](../../../../../../likelihood-function.md) by the normal intercept [prior distribution](../../../../../../prior-probability.md) gives

$$
\mathbb E(\alpha_i\mid\text{others},y)=w\overline r_i+(1-w)\delta,\qquad
w=\frac{3\tau^2}{\sigma^2+3\tau^2},
$$

with conditional [variance](../../../../../../variance-split.md) $(3/\sigma^2+1/\tau^2)^{-1}$. Thus small between-child variation produces stronger shrinkage towards $\delta$. The common mean and variation are themselves learned from all children in this [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
