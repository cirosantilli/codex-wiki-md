<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Consider the operators on all of $C_0(X)$ or $L^2(\mu)$, extending the displayed positive-function formula linearly. Here $C_0(X)$ is the [space of continuous functions vanishing at infinity](../../../../../space-of-continuous-functions-vanishing-at-infinity.md). The multiplier has modulus at most one, so $\|P_tf\|\leq\|f\|$, and multiplication of exponentials gives $P_{s+t}=P_sP_t$ and $P_0=I$. For [strong continuity](../../../../../strong-continuity.md) on $C_0(X)$, choose a compact $K$ outside which $|f|$ is small. On $K$ the continuous $k$ is bounded, making $e^{-tk}\to1$ uniform; outside $K$, $|(e^{-tk}-1)f|\leq|f|$. For $L^2(\mu)$, use [pointwise convergence](../../../../../pointwise-convergence.md) and the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) with bound $|(e^{-tk}-1)f|^2\leq|f|^2$. Thus both are [contraction semigroups](../../../../../contraction-semigroup.md), even when $k$ is unbounded.

The [generator of a multiplication semigroup](../../../../../generator-of-a-multiplication-semigroup.md) is

$$
\boxed{Lf=-kf,\qquad D_{C_0}(L)=\{f\in C_0(X):kf\in C_0(X)\},\qquad D_2(L)=\{f\in L^2(\mu):kf\in L^2(\mu)\}.}
$$

Indeed pointwise difference quotients converge to $-kf$. A [norm](../../../../../norm.md) limit therefore forces the displayed domain condition, using an almost-everywhere convergent subsequence for the $L^2$ case. Conversely $|(e^{-tk}-1)/t|\leq k$, so the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) proves the $L^2$ limit when $kf\in L^2$. In $C_0(X)$ write the error as $kf$ times $1-(1-e^{-tk})/(tk)$, with the value at $k=0$ supplied by continuity. That second factor tends uniformly to zero where $k$ is bounded and has modulus at most one; the compact-set and small-tail argument applied to $kf$ proves [uniform convergence](../../../../../uniform-convergence.md). To prove directly that $L$ is a [closed operator](../../../../../closed-linear-operator.md), take $f_n\to f$ and $Lf_n\to g$. Pointwise limits in $C_0$, or a common almost-everywhere convergent subsequence in $L^2$, give $g=-kf$. Thus $f$ is in the appropriate [generator domain](../../../../../generator-domain.md) and $Lf=g$. In $L^2$ the domain is dense because $f\mathbf1_{\{k\leq n\}}\to f$; in $C_0$ compactly supported [continuous functions](../../../../../continuous-function.md) are a dense subspace contained in the domain.

A real [multiplication operator](../../../../../multiplication-operator.md) on its maximal $L^2$ domain is an [unbounded self-adjoint operator](../../../../../unbounded-self-adjoint-operator.md). One direct verification is to test the adjoint relation against functions supported on $\{k\leq n\}$. If $h$ is in the [adjoint operator](../../../../../adjoint-operator.md) domain with representing vector $g$, those tests force $g=-kh$ on each such set, hence $kh\in L^2$. The converse follows by integration. On the [sigma-finite measure](../../../../../sigma-finite-measure.md) spaces used below, the [spectrum of a real multiplication operator](../../../../../spectrum-of-a-real-multiplication-operator.md) is its [essential range](../../../../../essential-range.md); spectral values are detected by [unit vectors](../../../../../unit-vector.md) supported where the multiplier is arbitrarily close to that value, while outside the essential range its reciprocal is a bounded resolvent multiplier.

For the [heat semigroup](../../../../../heat-semigroup.md) on $L^2(\mathbb R,dx)$, take the normalization $L_H=f''$. The unitary [Fourier transform](../../../../../fourier-transform.md) converts it to multiplication by $-\xi^2$, and converts the semigroup to multiplication by $e^{-t\xi^2}$. Consequently

$$
\boxed{D(L_H)=H^2(\mathbb R),\qquad\sigma(L_H)=(-\infty,0],\qquad L_H=L_H^*.}
$$

The [Sobolev space](../../../../../sobolev-space-split.md) domain is exactly $\{f:\xi^2\widehat f\in L^2\}$. The continuous [spectrum](../../../../../spectrum-functional-analysis.md) comes from the full [essential range](../../../../../essential-range.md) of $-\xi^2$, not from square-integrable Fourier [eigenvectors](../../../../../eigenvector.md).

For the [Ornstein-Uhlenbeck semigroup](../../../../../ornstein-uhlenbeck-semigroup.md) on standard [Gaussian measure](../../../../../gaussian-measure.md), the normalized [Probabilists' Hermite polynomials](../../../../../probabilists-hermite-polynomial.md) $h_n=\operatorname{He}_n/\sqrt{n!}$ form an [orthonormal basis](../../../../../orthonormal-basis.md). The construction below gives $L_{OU}=D^2-xD$ and $L_{OU}h_n=-nh_n$, so the Hermite coefficient map turns it into a real [multiplication operator](../../../../../multiplication-operator.md) on $\ell^2(\mathbb N_0)$. Therefore

$$
\boxed{D(L_{OU})=\left\{\sum_{n\geq0}c_nh_n:\sum_{n\geq0}n^2|c_n|^2<\infty\right\},\quad\sigma(L_{OU})=\{0,-1,-2,\ldots\},\quad L_{OU}=L_{OU}^*.}
$$

Finally, **the heat semigroup on the whole real line has no positive [spectral gap](../../../../../spectral-gap.md)**, whereas **the standard [Ornstein-Uhlenbeck semigroup](../../../../../ornstein-uhlenbeck-semigroup.md) has gap one**. For the first claim, take a nonzero smooth compactly supported $\phi$ and set $f_R(x)=R^{-1/2}\phi(x/R)$. Then $\|f_R\|_2^2=\|\phi\|_2^2$, but $\|f_R'\|_2^2=R^{-2}\|\phi'\|_2^2$. This disproves a uniform whole-line [Poincaré inequality](../../../../../poincare-inequality.md) $\|f\|_2^2\leq C\|f'\|_2^2$; one can also choose $\int\phi=0$. Lebesgue measure here is infinite, so it has no normalized probability mean to subtract. For [Gaussian measure](../../../../../gaussian-measure.md), the Hermite expansion instead gives the sharp [Gaussian Poincaré inequality](../../../../../gaussian-poincare-inequality.md)

$$
\boxed{\operatorname{Var}_\gamma(f)=\sum_{n\geq1}|c_n|^2\leq\sum_{n\geq1}n|c_n|^2=\int|f'|^2\,d\gamma.}
$$

Equality holds for affine functions. The identity on the right is interpreted on the energy-form domain, which is larger than the full [operator domain](../../../../../operator-domain.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
