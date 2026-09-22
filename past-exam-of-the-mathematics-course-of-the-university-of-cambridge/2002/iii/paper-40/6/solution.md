<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [linear filter of a stationary time series](../../../../../linear-filter-of-a-stationary-time-series.md) with real coefficients $(a_j)_{j\in\mathbb Z}$ satisfying $\sum_j|a_j|<\infty$ is $Y_t=\sum_ja_jX_{t-j}$. Its [filter generating function](../../../../../filter-generating-function.md) is the [Laurent series](../../../../../laurent-series.md) $A(z)=\sum_ja_jz^j$, absolutely convergent on $|z|=1$, and its [filter transfer function](../../../../../filter-transfer-function.md) is $H_A(\lambda)=A(e^{-i\lambda})$. For a one-sided filter this is a [power series](../../../../../power-series.md); a general two-sided filter need not converge on a larger annulus.

The filter theorem states that if $X$ is second-order stationary, then $Y$ exists in mean square, is second-order stationary, and has mean and [covariance](../../../../../covariance.md)

$$
\mathbb EY_t=\mu\sum_ja_j,\qquad
\gamma_Y(h)=\sum_{j,k}a_ja_k\gamma_X(h-j+k).
$$

Its [spectral measure of a stationary time series](../../../../../spectral-measure-of-a-stationary-time-series.md) is $dF_Y(\lambda)=|H_A(\lambda)|^2dF_X(\lambda)$. In particular, if $X$ has a [time-series spectral density](../../../../../spectral-density-of-a-stationary-process.md) in the convention $\gamma_X(h)=\int_{-\pi}^{\pi}e^{ih\lambda}f_X(\lambda)\,d\lambda$, then

$$
\boxed{f_Y(\lambda)=|A(e^{-i\lambda})|^2f_X(\lambda).}
$$

To prove existence, the $L^2$ norm of a tail of the filter is at most $\|X_0\|_2$ times the sum of the omitted $|a_j|$, which tends to zero. Hence finite partial sums converge in $L^2$. Expectations and [covariances](../../../../../covariance.md) pass to the limit, and the [covariance](../../../../../covariance.md) double sum is absolutely convergent because $|\gamma_X(h)|\leq\gamma_X(0)$. Its formula depends only on $h$, proving stationarity. Insert the spectral representation of $\gamma_X(h-j+k)$ and interchange sums and integration; the bound $\sum_{j,k}|a_ja_k|F_X([ -\pi,\pi])<\infty$ justifies the interchange. The resulting factor is $\sum_ja_je^{-ij\lambda}\sum_ka_ke^{ik\lambda}=|A(e^{-i\lambda})|^2$. This proves the spectral statement, including the [spectral density transformation under a linear filter](../../../../../spectral-density-transformation-under-a-linear-filter.md) without assuming that the input [autocovariances](../../../../../autocovariance.md) are absolutely summable.

For an [autoregressive moving-average model](../../../../../autoregressive-moving-average-model.md), use real polynomials normalized by $\phi_0=\theta_0=1$ and first work with the reduced noise-driven representation. If $\phi$ has no zero on the [unit circle](../../../../../complex-unit-circle.md), the rational function $C(z)=\theta(z)/\phi(z)$ has a Laurent expansion in an annulus containing that circle, with absolutely summable coefficients. Filtering the [white noise](../../../../../white-noise.md) with it gives a stationary solution. Its [time-series spectral density](../../../../../spectral-density-of-a-stationary-process.md) is

$$
\boxed{f_X(\lambda)=\frac{\sigma^2}{2\pi}\frac{|\theta(e^{-i\lambda})|^2}{|\phi(e^{-i\lambda})|^2},\qquad-\pi\leq\lambda\leq\pi.}
$$

Conversely, for coprime $\phi,\theta$, a unit-circle zero of $\phi$ would make this ratio nonintegrable, since the numerator does not vanish there; thus there is no finite-variance stationary noise-driven solution. A stationary solution can use a bilateral filter when autoregressive roots lie inside the [unit circle](../../../../../complex-unit-circle.md). The stronger causal condition, meaning dependence only on present and past noise, requires every zero of $\phi$ strictly outside the [unit disk](../../../../../unit-disk.md). Common factors must be handled before applying these conditions; a cancelled unit-root factor can also allow additional deterministic stationary components, which are outside the minimal noise-driven convention.

[Identifiability](../../../../../identifiability.md) means that different admissible parameters cannot produce the same stationary process law. In this zero-mean Gaussian setting, its law is determined by its [covariance](../../../../../covariance.md), equivalently its spectrum. Unrestricted [ARMA](../../../../../autoregressive-moving-average-model.md) coefficients are not identifiable from that law: if a moving-average factor has root $r$ inside the disk, then on $|z|=1$,

$$
|1-z/r|^2=|r|^{-2}|1-\overline r z|^2.
$$

Reflecting the root outside and multiplying the innovation [variance](../../../../../variance-split.md) by $|r|^{-2}$ preserves the spectrum, and therefore the Gaussian law. Common polynomial factors and arbitrary overall scaling give further redundancy. A regular canonical identifiable parameterization requires constant coefficients one, coprime polynomials of their stated minimal orders, all zeros of both $\phi$ and $\theta$ outside the closed [unit disk](../../../../../unit-disk.md), and $\sigma^2>0$.

Here is a proof of [canonical identifiability of Gaussian ARMA models](../../../../../canonical-identifiability-of-gaussian-arma-models.md). Suppose two such models have equal spectra and write their innovation standard deviations as $\sigma,\tau>0$. The ratio $R(z)=\sigma\theta(z)\widetilde\phi(z)/[\tau\widetilde\theta(z)\phi(z)]$ and its reciprocal are analytic on a neighbourhood of the closed [unit disk](../../../../../unit-disk.md), with modulus one on its boundary. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) applied to both makes $|R|=1$ throughout the disk, so $R$ is constant. Its value at zero is the positive number $\sigma/\tau$, forcing $R=1$ and $\sigma=\tau$. Therefore $\theta\widetilde\phi=\widetilde\theta\phi$; coprimality and the normalization at zero force equality of both polynomials. This proves the claimed parameter uniqueness within that canonical class.

In this class, $D(z)=\phi(z)/\theta(z)$ is analytic on a disk of radius greater than one. Its [Taylor series](../../../../../taylor-series.md) coefficients are absolutely summable, so

$$
\boxed{\varepsilon_t=D(B)X_t=\sum_{j\geq0}d_jX_{t-j}.}
$$

This is an [invertible time-series representation](../../../../../invertible-time-series-representation.md), proved by composition of the stable filters. Causality makes $\varepsilon_t$ orthogonal to past observations; invertibility makes past noises recoverable from past observations. Their closed past linear spans agree, so this noise is the linear innovation and the one-sided expansion $X_t=\sum_{j\geq0}c_j\varepsilon_{t-j}$ is the [Wold representation](../../../../../wold-decomposition.md). Mere stationarity without the stated canonical restrictions does not imply invertibility of the originally written noise representation.

For this one-sided canonical representation, $C(z)=\theta(z)/\phi(z)=\sum_{j\geq0}c_jz^j$. Comparing coefficients gives the [ARMA coefficient recursions](../../../../../arma-coefficient-recursions.md)

$$
\sum_{r=0}^{\min(p,k)}\phi_rc_{k-r}=\theta_k,\qquad c_j=0\ (j<0),\quad\theta_k=0\ (k>q).
$$

Thus for exactly the range asked for,

$$
\boxed{c_k+\phi_1c_{k-1}+\cdots+\phi_pc_{k-p}=0\quad(k>\max(p-1,q)).}
$$

The characteristic rates are reciprocals of the zeros of $\phi$. Partial fractions therefore express the tail as sums of $P_r(k)r^k$, where $|r|<1$ and the degree of $P_r$ is at most one less than the corresponding root multiplicity. Hence the coefficients decay exponentially, with possible polynomial and damped oscillatory factors. If $p=0$, they instead vanish after $q$. For a noncausal or noninvertible original specification, the Wold coefficients refer to the canonical spectral factor; using the original driving noise as the Wold innovation without checking these restrictions would be incorrect.

The [autocovariance](../../../../../autocovariance.md) is $\gamma(h)=\sigma^2\sum_{j\geq0}c_jc_{j+|h|}$. Analyticity of $C$ on a disk of radius $R>1$ gives $|c_j|\leq MR^{-j}$ for a slightly smaller radius than its first pole, and consequently $|\gamma(h)|\leq\sigma^2M^2R^{-|h|}/(1-R^{-2})$. Moreover, multiply the [ARMA](../../../../../autoregressive-moving-average-model.md) equation at time $t$ by $X_{t-h}$ and take expectations. For $h>q$, all noises $\varepsilon_{t-s}$ with $0\leq s\leq q$ are later than $X_{t-h}$ and orthogonal to it. For $h>\max(p-1,q)$ this gives

$$
\boxed{\gamma(h)+\phi_1\gamma(h-1)+\cdots+\phi_p\gamma(h-p)=0.}
$$

The [covariance](../../../../../covariance.md) tail therefore has the same characteristic exponential rates and multiplicity patterns as the filter coefficients, subject to possible cancellation of amplitudes. Pure moving averages have an exact [covariance](../../../../../covariance.md) cutoff.

For the final process, factor the polynomials:

$$
\phi(z)=1-\frac z3-\frac{2z^2}{9}=\left(1-\frac{2z}{3}\right)\left(1+\frac z3\right),\qquad
\theta(z)=1-\frac{2z}{3}.
$$

The common factor has its zero at $3/2$, so it can be cancelled as a stable filter. Explicitly, let $Y_t=(1+B/3)X_t-\varepsilon_t$; the original equation gives $Y_t=(2/3)Y_{t-1}$. The second moments of $Y_t$ are uniformly bounded because those of $X_t$ and $\varepsilon_t$ are. Iterating gives $Y_t=(2/3)^mY_{t-m}$, whose $L^2$ norm tends to zero as $m\to\infty$, so $Y_t=0$ in mean square. Thus

$$
X_t=-\frac13X_{t-1}+\varepsilon_t=\sum_{j\geq0}\left(-\frac13\right)^j\varepsilon_{t-j}.
$$

Summing the [covariance](../../../../../covariance.md) series gives

$$
\boxed{\gamma(h)=\frac{9\sigma^2}{8}\left(-\frac13\right)^{|h|},\qquad h\in\mathbb Z.}
$$

The process is a causal stationary [autoregressive process of order one](../../../../../autoregressive-process-of-order-one.md), with alternating-sign geometric [correlations](../../../../../pearson-correlation-coefficient.md), and is invertible. The displayed [ARMA](../../../../../autoregressive-moving-average-model.md)(2,1) description is nonminimal because of its common factor; its minimal identifiable class is [ARMA](../../../../../autoregressive-moving-average-model.md)(1,0).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
