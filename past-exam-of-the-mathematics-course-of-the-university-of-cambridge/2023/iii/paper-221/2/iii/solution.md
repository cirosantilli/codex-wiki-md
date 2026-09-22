<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Estimate the [propensity score](../../../../../../propensity-score.md) $\pi$ and the untreated outcome regression $\mu$, preferably with [cross-fitting](../../../../../../cross-fitting.md) when flexible methods are used, and set

$$
\widehat\beta
=\frac1n\sum_{i=1}^n\left[
(1-A_i)\frac{\widehat\pi(X_i)}{1-\widehat\pi(X_i)}
\{Y_i-\widehat\mu(X_i)\}
+A_i\widehat\mu(X_i)
\right].
$$

With $n_1=\sum_iA_i$, the resulting [one-step estimator](../../../../../../one-step-estimator.md) of the ATT is

$$
\widehat\tau_{\mathrm{ATT}}
=\frac1{n_1}\sum_iA_iY_i-\frac{\widehat\beta}{n_1/n}.
$$

Equivalently,

$$
\widehat\tau_{\mathrm{ATT}}
=\frac1{n_1}\sum_i\left[
A_i\{Y_i-\widehat\mu(X_i)\}
-(1-A_i)\frac{\widehat\pi(X_i)}{1-\widehat\pi(X_i)}
\{Y_i-\widehat\mu(X_i)\}
\right].
$$

This is an [augmented inverse-probability-weighted estimator](../../../../../../augmented-inverse-probability-weighted-estimator.md); it is consistent when either the propensity model or the untreated outcome model is correct, subject to the usual regularity and positivity conditions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
