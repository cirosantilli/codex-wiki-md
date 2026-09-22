<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Given numerical values of $\mu$ and $\sigma^2$, maximize the joint log-likelihood over the response rates $0<p_{jk}<1$:

$$
\sum_{j,k}\left[
S_{jk}\log p_{jk}+(n_{jk}-S_{jk})\log(1-p_{jk})
\right]
-\frac1{2\sigma^2}\sum_j
\left\{
\operatorname{logit}(p_{j1})-\operatorname{logit}(p_{j0})-\mu
\right\}^2.
$$

This is a penalized [binomial regression](../../../../../../../binomial-regression.md) problem and can be solved by [Newton method](../../../../../../../newton-s-method-in-optimization.md) or another numerical optimizer. One may alternate this maximization with the closed-form updates for $\mu$ and $\sigma^2$ from part i until convergence. The selected solution should have a negative-definite Hessian in the fitted log-odds parameters.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
