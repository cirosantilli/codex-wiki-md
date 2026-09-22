<h1 id="o/o5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gaussian linear model](../../../../../normal-linear-model-split.md) has log [likelihood function](../../../../../likelihood-function.md), up to an additive constant,

$$
\ell(\theta,\sigma^2)=-\frac n2\log\sigma^2-
\frac1{2\sigma^2}(Y-X\theta)^T(Y-X\theta).
$$

For each fixed positive $\sigma^2$, maximize this by minimizing the residual sum of squares. Differentiation gives the [normal equations](../../../../../normal-equations-for-linear-least-squares.md)

$$
X^TX\widehat\theta=X^TY.
$$

The full column rank of $X$ makes $X^TX$ [positive definite](../../../../../positive-definite-matrix.md), hence invertible, so

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY.}
$$

The quadratic objective is strictly convex, which proves uniqueness. The joint [maximum-likelihood estimate](../../../../../maximum-likelihood-estimation-split.md) has the same coefficient estimate, except on the [probability](../../../../../probability.md)-zero event of an exactly zero residual when the positive-[variance](../../../../../variance-split.md) likelihood has no finite joint maximizer.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
