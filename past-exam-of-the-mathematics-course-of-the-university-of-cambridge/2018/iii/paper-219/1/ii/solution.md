<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Independence makes the [variance of an estimator](../../../../../../variance-of-an-estimator.md) equal to

$$
\operatorname{Var}(\widehat\mu)=\alpha_1^2\sigma_1^2+\alpha_2^2\sigma_2^2.
$$

With $\alpha_2=1-\alpha_1$, differentiate to obtain $2\alpha_1\sigma_1^2-2(1-\alpha_1)\sigma_2^2=0$. The second derivative is $2(\sigma_1^2+\sigma_2^2)>0$, so the unique minimum is

$$
\boxed{\alpha_1=\frac{\sigma_2^2}{\sigma_1^2+\sigma_2^2},\qquad\alpha_2=\frac{\sigma_1^2}{\sigma_1^2+\sigma_2^2}}.
$$

Equivalently, the [inverse-variance weighted mean](../../../../../../inverse-variance-weighted-mean.md) uses $\alpha_i=K\sigma_i^\gamma$ with

$$
\boxed{\gamma=-2,\qquad K=(\sigma_1^{-2}+\sigma_2^{-2})^{-1},\qquad\operatorname{Var}(\widehat\mu)=\frac{\sigma_1^2\sigma_2^2}{\sigma_1^2+\sigma_2^2}}.
$$

We assume positive measurement [variances](../../../../../../variance-split.md). A zero-variance observation already supplies the true value exactly.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
