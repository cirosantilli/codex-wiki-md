<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Condition on the fixed [design matrix](../../../../../../design-matrix.md) and a prespecified $\lambda$. Put $M=G+n\lambda I_2$. The [covariance and bias of a ridge regression estimator](../../../../../../covariance-and-bias-of-a-ridge-regression-estimator.md) follow from its being a linear transformation of the response:

$$
\boxed{\operatorname{Cov}(\widehat\beta_\lambda)=\sigma^2M^{-1}GM^{-1},\qquad\operatorname{Var}(\widehat\beta_{j,\lambda})=\sigma^2[M^{-1}GM^{-1}]_{jj},\quad j=1,2.}
$$

Here centering the response introduces no correction in this expression because $X_s^T\mathbf1=0$. For the equal-norm two-predictor design, either diagonal entry simplifies to

$$
\operatorname{Var}(\widehat\beta_{j,\lambda})=\frac{\sigma^2}{2n}\left\{\frac{1+\rho}{(1+\rho+\lambda)^2}+\frac{1-\rho}{(1-\rho+\lambda)^2}\right\}.
$$

However,

$$
\mathbb E[\widehat\beta_\lambda]=M^{-1}G\beta,\qquad\operatorname{Bias}(\widehat\beta_\lambda)=-n\lambda M^{-1}\beta.
$$

**The variances quantify sampling variability, but alone do not give valid confidence intervals for the unshrunk slopes.** Centering a normal interval at the ridge estimate ignores its [bias](../../../../../../bias-of-an-estimator.md), which depends on the unknown slopes and need not be small relative to its standard error. Intervals require an appropriate bias correction, a bound on that bias, or another justified inferential procedure. A data-selected penalty introduces additional selection dependence not covered by the fixed-$\lambda$ formula. Similarly, holding a software penalty fixed while converting it using an estimated response scale does not hold the effective penalty fixed over repeated samples; the displayed covariance is not an unconditional variance formula for that nonlinear procedure.

## ↑ Ancestors (11)

1. [E](../e.md)
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
