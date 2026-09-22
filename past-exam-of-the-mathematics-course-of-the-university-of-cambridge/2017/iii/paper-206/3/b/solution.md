<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose knots independently of the eventual validation responses, and let $b(x)=(b_1(x),\ldots,b_K(x))^T$ be a [natural cubic spline](../../../../../../natural-cubic-spline.md) [basis](../../../../../../basis.md) as in part (a). A [regression spline](../../../../../../regression-spline.md) writes $m(x)=b(x)^T\beta$. Define the [design matrix](../../../../../../design-matrix.md) $B_{ij}=b_j(X_i)$. Under the stated [normal linear model](../../../../../../normal-linear-model.md), [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) for $\beta$ is the same as [ordinary least squares](../../../../../../ordinary-least-squares.md):

$$
\widehat\beta=\arg\min_\beta\|Y-B\beta\|^2.
$$

Differentiation gives the [normal equations](../../../../../../normal-equation.md) $B^TB\widehat\beta=B^TY$. If the design has full column rank,

$$
\boxed{\widehat m(x)=b(x)^T(B^TB)^{-1}B^TY.}
$$

If it does not, a [Moore-Penrose inverse](../../../../../../moore-penrose-inverse.md) gives the fitted values, but not every coefficient or off-sample prediction is identifiable. Merely choosing distinct knots does not guarantee full rank for an arbitrary set of observed predictor values.

More knots allow greater curvature and reduce approximation [bias](../../../../../../bias-of-an-estimator.md) at the cost of larger estimation [variance](../../../../../../variance-split.md). Too many or poorly located knots can cause unstable fits. Equally spaced knots are simple; empirical predictor [quantiles](../../../../../../quantile-function.md) put more flexibility where observations are dense; subject knowledge can concentrate knots near likely changes. Both the number and positions can be compared using [cross-validation](../../../../../../cross-validation.md) or an appropriate penalized model-selection criterion. Adaptive knot selection must be included within validation, since treating a data-selected basis as prespecified understates its flexibility. Boundary knots should cover the region where inference is intended, and natural linear tails do not by themselves justify far-out extrapolation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
