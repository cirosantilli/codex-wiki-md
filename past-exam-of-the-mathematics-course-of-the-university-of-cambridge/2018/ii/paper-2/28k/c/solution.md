<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Combining the Gaussian likelihood with the prior $\theta\sim N_p(0,c^2I_p)$ gives the posterior precision and mean

$$
I_p+c^{-2}I_p,
\qquad
\left(I_p+c^{-2}I_p\right)^{-1}X.
$$

Thus the posterior in the [Gaussian normal-mean shrinkage Bayes estimator](../../../../../../gaussian-normal-mean-shrinkage-bayes-estimator.md) is

$$
\theta\mid X
\sim N_p\left(
\frac{c^2}{1+c^2}X,
\frac{c^2}{1+c^2}I_p
\right).
$$

The [Bayes estimator under squared error loss](../../../../../../bayes-estimator-under-squared-error-loss.md) is the posterior mean, so

$$
\boxed{\widehat\theta_c(X)=\frac{c^2}{1+c^2}X.}
$$

Its posterior expected loss is the trace of the posterior covariance and does not depend on $X$. Therefore its [Bayes risk](../../../../../../bayes-risk.md) is

$$
\boxed{r(\pi_c)=\frac{pc^2}{1+c^2}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
