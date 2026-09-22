<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the two-sided [spectral density of a stationary process](../../../../../spectral-density-of-a-stationary-process.md) convention

$$
\boxed{\gamma_k=\int_{-\pi}^{\pi}e^{ik\lambda}f_X(\lambda)\,d\lambda.}
$$

Thus [white noise](../../../../../white-noise.md) of [variance](../../../../../variance-split.md) $\sigma^2$ has density $\sigma^2/(2\pi)$.

Absolute summability makes the [linear filter of a stationary time series](../../../../../linear-filter-of-a-stationary-time-series.md) well defined in $L^2$: $\sum_r\|a_rX_{t-r}\|_2\leq\|X_0\|_2\sum_r|a_r|<\infty$. Its [mean](../../../../../expected-value.md) is $m_Y=m_X\sum_ra_r$. For its [autocovariance](../../../../../autocovariance.md), continuity of the $L^2$ inner product gives

$$
\gamma_Y(k)=\sum_{r,s}a_ra_s\gamma_X(k-r+s).
$$

The sum is absolutely convergent because $|\gamma_X(j)|\leq\gamma_X(0)$. It depends only on $k$, proving [weak stationarity](../../../../../weakly-stationary-process.md). Inserting the spectral inversion formula and exchanging the absolutely dominated sum with the integral yields

$$
\begin{aligned}
\gamma_Y(k)&=\int_{-\pi}^{\pi}e^{ik\lambda}
 \left(\sum_ra_re^{-ir\lambda}\right)
 \left(\sum_sa_se^{is\lambda}\right)f_X(\lambda)\,d\lambda,\\
\boxed{f_Y(\lambda)}&=\boxed{|a(\lambda)|^2f_X(\lambda)}.
\end{aligned}
$$

Here the coefficients are real, so the two factors are complex conjugates. This is the [spectral density transformation under a linear filter](../../../../../spectral-density-transformation-under-a-linear-filter.md).

Applying a second [linear filter of a stationary time series](../../../../../linear-filter-of-a-stationary-time-series.md) gives

$$
\boxed{f_Z(\lambda)=|b(\lambda)|^2|a(\lambda)|^2f_X(\lambda).}
$$

The [composition of absolutely summable time-series filters](../../../../../composition-of-absolutely-summable-time-series-filters.md) can also be calculated directly:

$$
Z_t=\sum_jb_j\sum_ra_rX_{t-j-r}=\sum_\ell c_\ell X_{t-\ell},\qquad
\boxed{c_\ell=\sum_jb_ja_{\ell-j}.}
$$

Indeed $\sum_\ell|c_\ell|\leq\|a\|_1\|b\|_1$; this bound also justifies the interchange of the two $L^2$ sums. The [filter gain](../../../../../filter-gain.md) multiplies under this composition. The sketches for the two individual filters are:

<a id="2/image-ordinary-and-twelve-step-seasonal-difference-filter-gains"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47-filter-gains.png)

**[Figure 1](#2/image-ordinary-and-twelve-step-seasonal-difference-filter-gains). Ordinary and twelve-step seasonal difference-filter gains**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
