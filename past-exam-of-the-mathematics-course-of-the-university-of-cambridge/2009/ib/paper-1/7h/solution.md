<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

An [unbiased estimator](../../../../../unbiased-estimator.md) $\widehat\theta$ satisfies $\mathbb E_\theta\widehat\theta=\theta$ for every parameter value. Under the standard full-column-rank assumption on the [design matrix](../../../../../design-matrix.md), the Gaussian [log-likelihood](../../../../../log-likelihood.md) for the [normal linear model](../../../../../normal-linear-model.md), up to terms independent of $\beta$, is $-\|Y-X\beta\|^2/(2\sigma^2)$. Its maximum is the [ordinary least squares](../../../../../ordinary-least-squares.md) minimum. Differentiating gives $X^TX\widehat\beta=X^TY$, and full column rank makes $X^TX$ positive definite. Thus

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Since $\mathbb EY=X\beta$, its expectation is $(X^TX)^{-1}X^TX\beta=\beta$, proving **unbiasedness**. Estimating an unknown $\sigma^2$ as well does not change the maximizing coefficient vector.

The printed hypotheses give $p<n$ but do not explicitly require full column rank. Without that condition the [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md) are not unique: they are $X^+Y+z$ with $z\in\ker X$, as in [rank-deficient ordinary least squares](../../../../../rank-deficient-ordinary-least-squares.md). If $0\ne z\in\ker X$, the observation distributions at $\beta$ and $\beta+z$ are identical. Every estimator then has the same expectation at both parameters, so no estimator can be unbiased for both entire coefficient vectors. This proves [nonidentifiability prevents unbiased coefficient estimation](../../../../../nonidentifiability-prevents-unbiased-coefficient-estimation.md). The stated estimator and unbiasedness claim require the usual full-rank condition.

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
