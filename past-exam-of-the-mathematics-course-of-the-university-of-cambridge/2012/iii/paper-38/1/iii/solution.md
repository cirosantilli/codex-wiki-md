<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

In the usual causal stationary convention, a centered [autoregressive moving-average model](../../../../../../autoregressive-moving-average-model.md) satisfies

$$
X_t-\sum_{j=1}^p\phi_jX_{t-j}
=\varepsilon_t+\sum_{j=1}^q\theta_j\varepsilon_{t-j},
\qquad \varepsilon_t\sim\operatorname{WN}(0,\sigma^2).
$$

Set $\Phi(z)=1-\sum_{j=1}^p\phi_jz^j$ and $\Theta(z)=1+\sum_{j=1}^q\theta_jz^j$. After removal of common factors, the usual causality condition is that all zeros of $\Phi$ lie outside the closed unit disk. Then $\Theta(z)/\Phi(z)$ has an absolutely summable causal coefficient sequence, giving a linear-filter representation of $X$ in terms of [white noise](../../../../../../white-noise.md). Invertibility of the moving-average part is a separate issue and is not needed for its [covariance](../../../../../../covariance.md) spectrum.

[White noise](../../../../../../white-noise.md) has one-sided density $\sigma^2/\pi$. Applying the filtering result, or equating the spectra of the two filtered sides of the defining equation, gives

$$
\boxed{f_X(\omega)=\frac{\sigma^2}{\pi}
\frac{\left|1+\sum_{j=1}^q\theta_je^{ij\omega}\right|^2}
{\left|1-\sum_{j=1}^p\phi_je^{ij\omega}\right|^2}.}
$$

The moving-average sign agrees with the positive $\theta$ convention used later. More generally, the same quotient applies to a stationary two-sided solution when the reduced denominator has no unit-circle zeros; causality selects the past-dependent realization. This is the [spectral density of an ARMA process](../../../../../../spectral-density-of-an-arma-process.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
