# Likelihood-ratio test for an exponential support endpoint

↑ **Parent:** [Generalized likelihood-ratio test](generalized-likelihood-ratio-test.md)

Let $X_i=\theta+E_i$ for $n\geq2$ [independent and identically distributed](independent-and-identically-distributed-random-variables.md) observations, with $E_i$ having an [exponential distribution](exponential-distribution.md) of unknown scale $\beta>0$. Test the [null hypothesis](null-hypothesis.md) $\theta=0$ within $\theta\geq0$. For nondegenerate data, the [likelihood function](likelihood-function.md) is

$$
L(\theta,\beta)=\beta^{-n}\exp[-n(\overline X-\theta)/\beta]
\mathbf1_{\{0\leq\theta\leq X_{(1)}\}}.
$$

Maximizing over the scale gives $\widehat\beta(\theta)=\overline X-\theta$, and the resulting profile [likelihood](likelihood-function.md) increases with $\theta$. Thus the unrestricted [maximum-likelihood estimates](maximum-likelihood-estimator.md) are $\widehat\theta=X_{(1)}$ and $\widehat\beta=\overline X-X_{(1)}$, while the null estimate is $\widetilde\beta=\overline X$. The [likelihood ratio](likelihood-ratio.md) is consequently

$$
\boxed{R=\left(1-\frac{X_{(1)}}{\overline X}\right)^n.}
$$

Under the null, put $A=nX_{(1)}$ and $D=\sum_i(X_i-X_{(1)})$. The [memoryless property](memorylessness-of-the-exponential-distribution.md) gives independent [gamma distributions](gamma-distribution.md) of shapes $1$ and $n-1$ and common scale $\beta$. For a direct verification, fix which observation is the minimum and write its value as $z$ and the other observations as $z+e_j$. Their joint density is proportional to $e^{-nz/\beta}\prod_j e^{-e_j/\beta}$, which factors into an exponential density for the minimum and independent exponential densities for the excesses. The minimum's index does not affect the resulting laws of $A,D$.

By [beta sampling by gamma ratios](beta-sampling-by-gamma-ratios.md), $D/(A+D)\sim\operatorname{Beta}(n-1,1)$. Therefore

$$
\Pr_0(R\leq k)=k^{(n-1)/n},\qquad0\leq k\leq1.
$$

An exact [test size](size-of-a-statistical-test.md) $\alpha$ is obtained by rejecting for $R\leq\alpha^{n/(n-1)}$. Equivalently,

$$
\boxed{\frac{n-1}{n}(-2\log R)\sim\chi_2^2.}
$$

Although the alternative adds one endpoint parameter, a regular one-parameter [Wilks theorem](wilks-theorem.md) calibration is incorrect: the support depends on the endpoint, and the null lies on its boundary. In particular, $-2\log R$ tends to a [chi-squared distribution](chi-squared-distribution.md) with two [statistical degrees of freedom](statistical-degrees-of-freedom.md), not one.

## ↑ Ancestors (9)

1. [Generalized likelihood-ratio test](generalized-likelihood-ratio-test.md)
2. [Likelihood-ratio test](likelihood-ratio-test.md)
3. [Statistical hypothesis test](statistical-hypothesis-test-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2015/2/c/solution.md)
