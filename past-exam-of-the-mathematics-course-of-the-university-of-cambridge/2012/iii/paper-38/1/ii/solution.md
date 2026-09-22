<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The series defining the [linear filter of a stationary time series](../../../../../../linear-filter-of-a-stationary-time-series.md) converges in $L^2$, because the norm of a tail is at most $\|X_0\|_2$ times the corresponding tail sum of $|a_s|$. Its mean is the original mean times $\sum_s a_s$. Its [covariance](../../../../../../covariance.md) is time independent and equals

$$
\gamma_k^Y=\sum_{s,u\in\mathbb Z}a_sa_u\gamma_{k-s+u}.
$$

Under the summability assumption in (i),

$$
\sum_k|\gamma_k^Y|
\leq\left(\sum_s|a_s|\right)^2\sum_k|\gamma_k|<\infty.
$$

We may therefore interchange all the sums. Setting $h=k-s+u$ in the Fourier series gives

$$
\begin{aligned}
f_Y(\omega)
&=\frac1\pi\sum_{s,u}a_sa_u e^{i(s-u)\omega}
\sum_h\gamma_he^{ih\omega}\\
&=\left(\sum_sa_se^{is\omega}\right)
\left(\sum_ua_ue^{-iu\omega}\right)f_X(\omega).
\end{aligned}
$$

The second factor is the conjugate of the first because the coefficients are real. Hence

$$
\boxed{f_Y(\omega)=|\alpha(\omega)|^2f_X(\omega).}
$$

This [spectral density transformation under a linear filter](../../../../../../spectral-density-transformation-under-a-linear-filter.md) also holds whenever the original spectral measure has a density, without [covariance](../../../../../../covariance.md) summability: insert its integral representation into the [covariance](../../../../../../covariance.md) double sum, justified by absolute summability of the filter coefficients.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
