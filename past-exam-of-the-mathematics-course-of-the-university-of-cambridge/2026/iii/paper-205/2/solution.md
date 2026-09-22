<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [tower property of conditional expectation](../../../../../law-of-total-expectation.md) gives

$$
\mathbb E\!\left[\frac{YT}{\pi(X)}\middle|X\right]
=\frac{\mathbb E[YT\mid X]}{\pi(X)}
=\frac{\pi(X)\mu(X)}{\pi(X)}=\mu(X),
$$

and another expectation gives $\theta$.

Use the [augmented inverse-probability-weighted estimator](../../../../../augmented-inverse-probability-weighted-estimator.md)

$$
\widehat\theta_n=\frac1n\sum_{i=1}^n
\left[\widehat\mu_n(X_i)+\frac{T_i}{\widehat\pi_n(X_i)}
\{Y_i-\widehat\mu_n(X_i)\}\right].
$$

Condition on the independently trained nuisance estimators. Subtracting the oracle influence variable

$$
\phi(X,Y,T)=\mu(X)+\frac{T}{\pi(X)}(Y-\mu(X))
$$

produces a conditional empirical fluctuation with variance $o(1)$ after multiplication by $\sqrt n$, using $\mathcal E_\mu,\mathcal E_\pi\to0$, overlap, and the bounded conditional variance. Its conditional bias is

$$
\mathbb E\left[(\widehat\mu_n(X)-\mu(X))
\left(1-\frac{\pi(X)}{\widehat\pi_n(X)}\right)\right],
$$

whose absolute value is at most $\sqrt{\mathcal E_\mu\mathcal E_\pi}=o(n^{-1/2})$ by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Thus

$$
\sqrt n(\widehat\theta_n-\theta)
=\frac1{\sqrt n}\sum_{i=1}^n(\phi_i-\theta)+o_P(1).
$$

The [central limit theorem](../../../../../central-limit-theorem.md) and [Slutsky theorem](../../../../../slutsky-theorem.md) give the claimed $N(0,v)$ limit. Without auxiliary data, use [cross-fitting](../../../../../cross-fitting.md): split the sample into folds, train both nuisance estimators away from each observation's fold, and average the same score over held-out observations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
