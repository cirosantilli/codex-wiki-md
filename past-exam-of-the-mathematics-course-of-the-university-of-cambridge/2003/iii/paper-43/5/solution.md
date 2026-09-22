<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $C_j=\sum_{t=1}^T y_t\cos(\omega_jt)$ and $S_j=\sum_{t=1}^T y_t\sin(\omega_jt)$. The [discrete Fourier transform](../../../../../discrete-fourier-transform.md) coefficient is $C_j-iS_j$. Alternatively, by the given orthogonality relations, the harmonic obtained by [linear least-squares projection](../../../../../linear-least-squares-projection.md) has coefficients $a_j=2C_j/T$ and $b_j=2S_j/T$. Thus the source's [periodogram](../../../../../periodogram.md) is the squared amplitude of a fitted harmonic, scaled as power per unit angular frequency:

$$
I(\omega_j)=\frac{C_j^2+S_j^2}{\pi T}=\frac{T}{4\pi}(a_j^2+b_j^2).
$$

It measures how much of the centered record varies at frequency $\omega_j$. For odd $T$, Fourier [Parseval identity](../../../../../parseval-identity.md) gives

$$
\frac1T\sum_{t=1}^T(y_t-\bar y)^2=\frac{2\pi}{T}\sum_{j=1}^m I(\omega_j).
$$

The positive-frequency spacing is $2\pi/T$, so summing the power ordinates times this spacing estimates the total [variance](../../../../../variance-split.md). The factor $1/(\pi T)$ corresponds to the [one-sided spectral density](../../../../../one-sided-spectral-density-of-a-real-stationary-time-series.md) on $(0,\pi)$; the usual two-sided periodogram is half as large.

If the observations are [Gaussian white noise](../../../../../gaussian-white-noise.md) with common variance $\sigma^2$, the $2m$ harmonic sums are jointly [normally distributed](../../../../../normal-distribution.md). Their means are zero even with a nonzero constant series mean, because each sine and cosine sums to zero. Orthogonality gives

$$
\operatorname{Cov}(C_j,C_k)=\operatorname{Cov}(S_j,S_k)=\frac{T\sigma^2}{2}\delta_{jk},\qquad \operatorname{Cov}(C_j,S_k)=0.
$$

Uncorrelated coordinates of a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) are independent. Therefore all $C_j/\sqrt{T\sigma^2/2}$ and $S_j/\sqrt{T\sigma^2/2}$ are independent standard normals, and

$$
\boxed{I(\omega_j)\ \text{are independent with law}\ \frac{\sigma^2}{\pi}\frac{\chi_2^2}{2}.}
$$

Since the [chi-squared distribution](../../../../../chi-squared-distribution.md) with two degrees of freedom has mean two and variance four,

$$
\boxed{E[I(\omega_j)]=\sigma^2/\pi=f_+(\omega_j),\qquad\operatorname{Var}(I(\omega_j))=(\sigma^2/\pi)^2.}
$$

Here $f_+$ is the one-sided white-noise [spectral density](../../../../../spectral-density-of-a-stationary-process.md). Its exact unbiasedness is accompanied by a nonconcentrating distribution: along Fourier frequencies tending to any interior frequency, $I/f_+$ has the same nondegenerate exponential law at every $T$. It therefore does not converge in probability to one, proving failure of [statistical consistency](../../../../../consistency-statistics.md), not just nonvanishing variance.

For a general stationary process, exact finite-sample unbiasedness is not implied. Expanding the Fourier square instead gives

$$
E[I_T(\omega_j)]=\frac1\pi\sum_{h=-(T-1)}^{T-1}\left(1-\frac{|h|}{T}\right)\gamma(h)e^{-ih\omega_j},
$$

where $\gamma$ is the [autocovariance function](../../../../../autocovariance.md). Under suitable short-memory regularity this tends to $f_+(\omega)$ at frequencies $\omega_j\to\omega$. The periodogram is thus generally asymptotically unbiased, while the exact assertion above is for white noise.

Use [local periodogram smoothing](../../../../../local-periodogram-smoothing.md) to reduce variance: average $L_T$ neighboring ordinates with weights summing to one, where $L_T\to\infty$ but $L_T/T\to0$. At an interior frequency the shrinking frequency window makes the bias tend to zero for smooth $f_+$, while averaging many weakly dependent ordinates makes the variance of order $1/L_T$. For white noise with equal weights, the ordinates are exactly independent and the variance is exactly $f_+^2/L_T$. For a general process, impose suitable short-memory and fourth-order dependence assumptions, such as a stationary Gaussian model with sufficiently summable autocovariances. These conditions, together with smoothness, give a consistent smoothed estimator. Boundary frequencies require an appropriately one-sided or reflected window.

Smooth spectral density alone is not enough. For example let $y_t=A\epsilon_t$, where $A>0$ is a nondegenerate random variable constant throughout the record, independent of independent unit-variance Gaussian $\epsilon_t$, with $E[A^2]<\infty$. The unconditional [autocovariance](../../../../../autocovariance.md) is zero off lag zero and its one-sided [spectral density](../../../../../spectral-density-of-a-stationary-process.md) is the smooth constant $E[A^2]/\pi$. Nevertheless a long local average estimates the realized $A^2/\pi$, not that deterministic unconditional value. This nonergodic example explains why a dependence/ergodicity condition accompanies the smoothing argument.

For the [turning point test of randomness](../../../../../turning-point-test-of-randomness.md), the null is independent identically distributed continuous observations. Let $J_t$ be one if $y_t$ is a strict local maximum or minimum among $y_{t-1},y_t,y_{t+1}$, for $2\le t\le T-1$, and set $P_T=\sum_tJ_t$. Three ranks are equally likely; the middle observation is an extremum in four of the six orders, giving $E[J_t]=2/3$ and $\operatorname{Var}(J_t)=2/9$. Therefore

$$
\boxed{E[P_T]=\frac{2(T-2)}3.}
$$

Indicators more than two positions apart depend on disjoint observations and are independent. For neighboring indicators, both are one precisely when four observations alternate up-down-up or down-up-down. By the probability-integral transform, use four independent uniforms. The first pattern has probability

$$
\int_0^1\int_0^b b(1-c)\,dc\,db=\frac5{24};
$$

here $b=y_t$, $c=y_{t+1}<b$, with the two outer inequalities having probabilities $b$ and $1-c$. The reverse pattern has the same probability, so $E[J_tJ_{t+1}]=5/12$ and $\operatorname{Cov}(J_t,J_{t+1})=5/12-4/9=-1/36$.

At separation two, the triples share only one endpoint value $c$. Conditional on it, their other observations are independent. The probability that either triple's central observation is a turning point is

$$
r(c)=\int_c^1 b\,db+\int_0^c(1-b)\,db=\frac12+c-c^2.
$$

It follows that $E[J_tJ_{t+2}]=\int_0^1r(c)^2\,dc=9/20$, so this covariance is $9/20-4/9=1/180$. Combining all terms for $T\ge4$ gives

$$
\begin{aligned}
\operatorname{Var}(P_T)&=(T-2)\frac29+2(T-3)\left(-\frac1{36}\right)+2(T-4)\frac1{180}\\
&=\boxed{\frac{16T-29}{90}}.
\end{aligned}
$$

The standardized count is approximately standard normal for large $T$, by a [central limit theorem](../../../../../central-limit-theorem.md) for bounded 2-dependent indicators. A two-sided randomness test rejects for large absolute values of

$$
Z_T=\frac{P_T-2(T-2)/3}{\sqrt{(16T-29)/90}}.
$$

Too few turns suggests persistent movement, while too many suggests alternation. Exact rank-permutation calibration is possible at small $T$. Ties invalidate the continuous-rank probabilities unless their handling is specified. The test probes this feature of randomness; nonrejection does not establish independence.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
