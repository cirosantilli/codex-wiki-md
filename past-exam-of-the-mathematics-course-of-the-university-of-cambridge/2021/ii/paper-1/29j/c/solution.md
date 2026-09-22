<h1 id="29j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The model factors into the [normal distribution](../../../../../../normal-distribution.md) densities

$$
X_1\sim N(\theta,1)
$$

and, conditionally on $X_{i-1}$,

$$
X_i\mid X_{i-1}
\sim N\!\left(
\theta(1-\sqrt\gamma)+\sqrt\gamma X_{i-1},
1-\gamma
\right).
$$

Ignoring constants independent of $\theta$, the log likelihood is

$$
\ell_n(\theta)
=-\frac12(X_1-\theta)^2
-\frac1{2(1-\gamma)}
\sum_{i=2}^n
\left[
X_i-\sqrt\gamma X_{i-1}
-\theta(1-\sqrt\gamma)
\right]^2.
$$

Its score is

$$
S_n(\theta)
=(X_1-\theta)
+\frac{1-\sqrt\gamma}{1-\gamma}
\sum_{i=2}^n
\left[
X_i-\sqrt\gamma X_{i-1}
-\theta(1-\sqrt\gamma)
\right].
$$

In terms of the independent innovations,

$$
S_n(\theta)
=\varepsilon_1
+\frac{1-\sqrt\gamma}{\sqrt{1-\gamma}}
\sum_{i=2}^n\varepsilon_i.
$$

[Variance additivity for independent random variables](../../../../../../variance-additivity-for-independent-random-variables.md) therefore yields

$$
\boxed{
I_n(\theta)
=1+(n-1)\frac{(1-\sqrt\gamma)^2}{1-\gamma}
=1+(n-1)\frac{1-\sqrt\gamma}{1+\sqrt\gamma}}.
$$

Since $I_1(\theta)=1$, the equality $I_n=nI_1$ holds for all $n$ exactly when

$$
\frac{1-\sqrt\gamma}{1+\sqrt\gamma}=1,
$$

namely when

$$
\boxed{\gamma=0}.
$$

Thus the information tensorizes only in the independent case.

Finally, the [Cramér-Rao bound](../../../../../../cramer-rao-bound.md) gives every unbiased estimator $\widehat\theta$ the lower bound

$$
\boxed{
\operatorname{Var}_\theta(\widehat\theta)
\geq
\frac1{I_n(\theta)}
=\left[
1+(n-1)\frac{1-\sqrt\gamma}{1+\sqrt\gamma}
\right]^{-1}}.
$$

This is the [Fisher information in a stationary Gaussian autoregressive location model](../../../../../../fisher-information-in-a-stationary-gaussian-autoregressive-location-model.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
