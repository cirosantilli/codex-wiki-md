<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For an [orthonormal wavelet](../../../../../orthonormal-wavelet.md) construction, set

$$
\phi_{j,k}(x)=2^{j/2}\phi(2^jx-k),\qquad \psi_{j,k}(x)=2^{j/2}\psi(2^jx-k),\qquad k\in\mathbb Z.
$$

The [scaling function](../../../../../scaling-function.md) $\phi$ generates the approximation spaces $V_j$, while $\psi$ generates the detail spaces $W_j$ in the [multiresolution analysis](../../../../../multiresolution-analysis.md), with $V_{j+1}=V_j\oplus W_j$. At coarse resolution zero, the family $\{\phi_{0,k}\}_k\cup\{\psi_{j,k}\}_{j\geq0,k}$ is an [orthonormal basis](../../../../../orthonormal-basis.md) of $L^2(\mathbb R)$.

For the given square-integrable function the coefficients and [wavelet series](../../../../../wavelet-series.md) are

$$
a_{0,k}=\int_{\mathbb R}m(x)\phi_{0,k}(x)dx,\qquad b_{j,k}=\int_{\mathbb R}m(x)\psi_{j,k}(x)dx,
$$



$$
\boxed{m=\sum_{k\in\mathbb Z}a_{0,k}\phi_{0,k}+\sum_{j=0}^\infty\sum_{k\in\mathbb Z}b_{j,k}\psi_{j,k}.}
$$

For real [wavelets](../../../../../wavelet.md) these are the real [L2 inner products](../../../../../l2-inner-product.md); use complex conjugates for a complex basis. The series converges in the [L2 norm](../../../../../l2-norm.md), and its coefficients satisfy the [Parseval identity for a Hilbertian basis](../../../../../parseval-identity-for-a-hilbertian-basis.md)

$$
\|m\|_2^2=\sum_k|a_{0,k}|^2+\sum_{j\geq0,k}|b_{j,k}|^2.
$$

An $L^2$ hypothesis alone does not assert pointwise convergence.

The resolution-$J$ [wavelet projection](../../../../../wavelet-projection.md) is the [orthogonal projection](../../../../../orthogonal-projection.md) onto $V_J$:

$$
\boxed{P_Jm=\sum_ka_{0,k}\phi_{0,k}+\sum_{j=0}^{J-1}\sum_kb_{j,k}\psi_{j,k}=\sum_ka_{J,k}\phi_{J,k},\qquad a_{J,k}=\langle m,\phi_{J,k}\rangle.}
$$

The two expressions coincide by iterating $V_{j+1}=V_j\oplus W_j$. [Orthogonality](../../../../../orthogonal-vectors.md) gives $\|m-P_Jm\|_2^2=\sum_{j\geq J,k}|b_{j,k}|^2$, which tends to zero. One can equivalently write the projection with kernel $A_J(x,y)=\sum_k\phi_{J,k}(x)\phi_{J,k}(y)$, interpreted as the same [orthogonal projection](../../../../../orthogonal-projection.md).

In [fixed-design nonparametric regression](../../../../../fixed-design-nonparametric-regression.md), the observations satisfy

$$
\boxed{Y_i=m(x_i)+\varepsilon_i,\qquad x_i\text{ deterministic},\qquad \mathbb E\varepsilon_i=0,\quad \operatorname{Var}(\varepsilon_i)=\sigma^2,}
$$

with independent errors. In the usual Gaussian version $\varepsilon_i\sim N(0,\sigma^2)$. The [regression function](../../../../../regression-function.md) is evaluated at the design sites, so it must be specified pointwise there, not only as an $L^2$ equivalence class. For $x_i=i/n$, the observations concern $m$ on $[0,1]$. They cannot identify its values outside this interval. Use an [interval-adapted wavelet basis](../../../../../interval-adapted-wavelet-basis.md) on $[0,1]$, consisting of coarse functions $\phi_{0,k}$ and detail functions $\psi_{j,k}$; a [Haar wavelet](../../../../../haar-wavelet.md) basis is one explicit choice.

Here is a [wavelet regression estimator](../../../../../wavelet-regression-estimator.md) valid for every $n$. Divide $[0,1]$ into cells $I_i=((i-1)/n,i/n]$, with the value at zero assigned arbitrarily, and form the observed step function $\widetilde Y_n(t)=Y_i$ on $I_i$. For any normalized basis function $b_\lambda$, estimate its coefficient by

$$
\widehat c_\lambda=\int_0^1\widetilde Y_n(t)b_\lambda(t)dt=\sum_{i=1}^nw_{\lambda i}Y_i,\qquad w_{\lambda i}=\int_{I_i}b_\lambda(t)dt.
$$

The [wavelet regression estimator](../../../../../wavelet-regression-estimator.md) at resolution $J=J_n$ is therefore

$$
\boxed{\widehat m_J(t)=\sum_k\widehat a_{0,k}\phi_{0,k}(t)+\sum_{j=0}^{J-1}\sum_k\widehat b_{j,k}\psi_{j,k}(t)=P_J\widetilde Y_n(t).}
$$

Only finitely many interval basis functions occur. Its [expectation](../../../../../expected-value.md) is $P_Jm_n^{\mathrm{grid}}$, where $m_n^{\mathrm{grid}}$ equals $m(i/n)$ on $I_i$. Thus approximation of $m$ includes the resolution bias and the grid discretization bias. For continuous $m$, the latter tends uniformly to zero by [uniform continuity](../../../../../uniform-continuity.md). No smoothness or consistency claim for arbitrary pointwise representatives of $L^2$ functions is needed to define the estimator.

The common point-evaluation version replaces each weight by $b_\lambda(i/n)/n$, giving

$$
\widehat a_{0,k}=\frac1n\sum_iY_i\phi_{0,k}(i/n),\qquad \widehat b_{j,k}=\frac1n\sum_iY_i\psi_{j,k}(i/n).
$$

These are Riemann-sum approximations to the coefficient integrals. For [Haar wavelets](../../../../../haar-wavelet.md), $n=2^L$, and $J\leq L$, they equal the integrated-weight coefficients exactly if the dyadic cells and pointwise basis versions are chosen right-closed. Each retained basis function is then constant on every sampling cell. This gives a concrete implementation by the [discrete wavelet transform](../../../../../discrete-wavelet-transform.md). A sensible finest resolution has $2^J\leq n$; beyond the grid scale there are details the data cannot resolve.

For [wavelet coefficient thresholding](../../../../../wavelet-coefficient-thresholding.md), retain the coarse coefficients but discard detail coefficients dominated by noise. A hard-threshold version is

$$
\boxed{\widehat m^{\mathrm{thr}}_J=\sum_k\widehat a_{0,k}\phi_{0,k}+\sum_{j<J,k}\widehat b_{j,k}\mathbf1_{\{|\widehat b_{j,k}|>\tau_{j,k}\}}\psi_{j,k}.}
$$

Alternatively, [soft thresholding](../../../../../soft-thresholding.md) replaces each detail coefficient by $\operatorname{sgn}(\widehat b)(|\widehat b|-\tau)_+$. The unthresholded [wavelet regression estimator](../../../../../wavelet-regression-estimator.md) retains all details at the chosen resolution; thresholding retains evidence for local features while suppressing small fluctuations.

The thresholds can be derived from a [simultaneous wavelet coefficient noise bound](../../../../../simultaneous-wavelet-coefficient-noise-bound.md). Write $q_\lambda^2=\sum_iw_{\lambda i}^2$. Independence gives

$$
\operatorname{Var}(\widehat c_\lambda)=\sigma^2q_\lambda^2,\qquad q_\lambda^2\leq\frac1n\int_0^1b_\lambda(t)^2dt=\frac1n,
$$

where the inequality applies the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on each cell of length $1/n$. In the dyadic Haar implementation, $q_\lambda^2=1/n$ exactly. For Gaussian errors, the normalized coefficient noise is standard normal. More generally, independent centred [sub-Gaussian random variables](../../../../../sub-gaussian-distribution.md) with parameter $\sigma$ give

$$
\mathbb P\bigl(|\widehat c_\lambda-\mathbb E\widehat c_\lambda|>t\bigr)\leq2\exp\!\left(-\frac{t^2}{2\sigma^2q_\lambda^2}\right).
$$

If $N_J$ detail coefficients are considered, a [union bound](../../../../../boole-s-inequality.md) consequently justifies

$$
\boxed{\tau_\lambda=\sigma q_\lambda\sqrt{2\log(2N_J/\delta)}.}
$$

With [probability](../../../../../probability.md) at least $1-\delta$, every retained detail's noise is below its corresponding threshold; independence between the coefficient errors is unnecessary. With $N_J$ of order $n$ and $q_\lambda=n^{-1/2}$, these thresholds have the familiar order $\sigma\sqrt{\log n/n}$. Coefficients larger than their noise level represent potential signal, and a coefficient zero in the discretized mean is not selected on this simultaneous event. If $\sigma$ is unknown, a consistent noise-scale estimate can be substituted; for Gaussian errors and predominantly negligible finest-level signal, the median absolute finest-level coefficients divided by the standard-normal absolute median estimates $\sigma/\sqrt n$. Without a Gaussian or sub-Gaussian tail assumption, finite variance alone does not justify the logarithmic thresholds: [Chebyshev inequality](../../../../../chebyshev-inequality.md) and the [union bound](../../../../../boole-s-inequality.md) instead permit $\tau_\lambda=\sigma q_\lambda\sqrt{N_J/\delta}$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
