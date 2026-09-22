<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the [Gaussian white noise model](../../../../../gaussian-white-noise-model.md), observe the entire path

$$
\boxed{Y(t)=\int_0^tf(s)\,ds+n^{-1/2}W(t),\qquad0\leq t\leq1,}
$$

where $W$ is standard [Brownian motion](../../../../../brownian-motion-split.md) and the deterministic drift belongs to [L2 space](../../../../../l2-space-is-a-hilbert-space.md) on $[0,1]$. Equivalently, $dY(t)=f(t)\,dt+n^{-1/2}dW(t)$. For every deterministic $h\in L^2[0,1]$, the observed [stochastic integral](../../../../../stochastic-integral.md) satisfies

$$
Y(h):=\int_0^1h(t)\,dY(t)=\langle h,f\rangle+n^{-1/2}W(h),\qquad \operatorname{Cov}(W(h),W(g))=\langle h,g\rangle.
$$

The noise $W(h)=\int h\,dW$ is an [isonormal Gaussian process](../../../../../isonormal-gaussian-process.md). In particular its [variance](../../../../../variance-split.md) is $\|h\|_2^2$. [Gaussian white noise](../../../../../gaussian-white-noise.md) is interpreted through these integrals, rather than as an ordinary random [function](../../../../../function-split.md) with a pointwise value at every time. No smoothness of $f$ is needed.

Here is the [Gaussian maximum bound without independence](../../../../../gaussian-maximum-bound-without-independence.md). Put $M=\max_{1\leq i\leq N}|g_i|$. It is integrable since it is bounded by $\sum_i|g_i|$. For every $\lambda>0$,

$$
e^{\lambda M}\leq\sum_{i=1}^N\left(e^{\lambda g_i}+e^{-\lambda g_i}\right),\qquad E e^{\lambda M}\leq2N e^{\lambda^2/2}.
$$

The second inequality uses only the [moment-generating function](../../../../../moment-generating-function.md) of the [standard normal distribution](../../../../../standard-normal-distribution.md), so [independence](../../../../../independent-random-variables.md) is unnecessary. [Jensen inequality](../../../../../jensen-s-inequality.md) gives $e^{\lambda EM}\leq E e^{\lambda M}$, hence

$$
EM\leq\frac{\log(2N)}\lambda+\frac\lambda2.
$$

Minimizing at $\lambda=\sqrt{2\log(2N)}$ proves

$$
\boxed{E\max_{1\leq i\leq N}|g_i|\leq\sqrt{2\log(2N)}.}
$$

For the [dyadic partition](../../../../../dyadic-partition.md), let $I_{J,k}=[k2^{-J},(k+1)2^{-J})$, $0\leq k<2^J$, putting the endpoint $1$ into the final interval. The [Haar scaling functions](../../../../../haar-scaling-function.md)

$$
\phi_{J,k}=2^{J/2}\mathbf1_{I_{J,k}}
$$

form an [orthonormal basis](../../../../../orthonormal-basis.md) of the space $V_J$ of [functions](../../../../../function-split.md) constant on each interval. The [Haar wavelets](../../../../../haar-wavelet.md) can be written as

$$
\psi_{j,k}=2^{j/2}\left(\mathbf1_{I_{j+1,2k}}-\mathbf1_{I_{j+1,2k+1}}\right).
$$

For $J\geq1$, the constant [function](../../../../../function-split.md) $\phi_{0,0}=1$ together with $\psi_{j,k}$, $0\leq j<J$, is another [orthonormal basis](../../../../../orthonormal-basis.md) of $V_J$. Indeed, each successive level splits a cell's two constants into their sum and difference; the number of basis elements is $1+\sum_{j=0}^{J-1}2^j=2^J$. Thus the [Haar projection](../../../../../haar-projection.md) is the [orthogonal projection](../../../../../orthogonal-projection.md)

$$
\begin{aligned}
\Pi_{V_J}f&=\sum_{k=0}^{2^J-1}\langle f,\phi_{J,k}\rangle\phi_{J,k}\\
&=\langle f,1\rangle\,1+\sum_{j=0}^{J-1}\sum_{k=0}^{2^j-1}\langle f,\psi_{j,k}\rangle\psi_{j,k}.
\end{aligned}
$$

On cell $I_{J,k}$ its value is $2^J\int_{I_{J,k}}f(t)\,dt$. The first formula also applies to $J=0$.

Estimate each coefficient by its observed [stochastic integral](../../../../../stochastic-integral.md):

$$
\widehat\alpha_{J,k}=\int_0^1\phi_{J,k}(t)\,dY(t)=2^{J/2}\left[Y((k+1)2^{-J})-Y(k2^{-J})\right],\qquad\widehat\Pi_{V_J}f=\sum_k\widehat\alpha_{J,k}\phi_{J,k}.
$$

This is the [Haar projection estimator in Gaussian white noise](../../../../../haar-projection-estimator-in-gaussian-white-noise.md). The noise integrals over disjoint intervals form a [Gaussian vector](../../../../../gaussian-random-vector.md) with zero off-diagonal [covariance](../../../../../covariance.md). The principle that [uncorrelated jointly Gaussian variables are independent](../../../../../uncorrelated-jointly-normal-variables-are-independent.md) then makes these coefficients [independent](../../../../../independent-random-variables.md). Therefore

$$
\widehat\alpha_{J,k}=\langle f,\phi_{J,k}\rangle+n^{-1/2}Z_k,\qquad Z_k\overset{\mathrm{iid}}\sim N(0,1).
$$

Taking [expectations](../../../../../expected-value.md) shows that **$\widehat\Pi_{V_J}f$ is an [unbiased estimator](../../../../../unbiased-estimator.md) of $\Pi_{V_J}f$**, both coefficientwise and pointwise for the stated step-function representatives.

Only one scaling [function](../../../../../function-split.md) is nonzero in each cell, so the [supremum norm](../../../../../supremum-norm.md) of the error has the exact form

$$
\left\|\widehat\Pi_{V_J}f-\Pi_{V_J}f\right\|_\infty=\sqrt{\frac{2^J}{n}}\max_{0\leq k<2^J}|Z_k|.
$$

The endpoint convention ensures the same identity at $1$. Apply the [Gaussian maximum bound without independence](../../../../../gaussian-maximum-bound-without-independence.md) with $N=2^J$ to obtain the [supremum norm risk of a Haar projection estimator](../../../../../supremum-norm-risk-of-a-haar-projection-estimator.md):

$$
\boxed{E\left\|\widehat\Pi_{V_J}f-\Pi_{V_J}f\right\|_\infty\leq\sqrt{\frac{2^J}{n}}\sqrt{2\log(2^{J+1})}=\sqrt{\frac{2^J(2J+2)\log2}{n}}.}
$$

The factor $2^{J/2}$ comes from cellwise scaling, while the extra square root of $J+1$ comes from taking the maximum over $2^J$ Gaussian errors.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
