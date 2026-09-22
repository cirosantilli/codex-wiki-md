<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $a_0$ be the constant [Fourier coefficient](../../../../../fourier-coefficient.md) and suppose first that $k>0$ is even and $M_k\ne0$; thus $k\geq4$. Put $\varepsilon=i^k=(-1)^{k/2}$. The precise [Mellin continuation of a noncuspidal modular form](../../../../../mellin-continuation-of-a-noncuspidal-modular-form.md) is

$$
\boxed{\Lambda_f(s)=(2\pi)^{-s}\Gamma(s)L(f,s),\qquad
\Lambda_f(s)=\varepsilon\Lambda_f(k-s).}
$$

It is [meromorphic](../../../../../meromorphic-function.md) on the whole plane, with possible simple [poles](../../../../../pole.md) only at $0,k$, of residues $-a_0,\varepsilon a_0$, respectively. For a [cusp form](../../../../../cusp-form.md) it is an [entire function](../../../../../entire-function.md). A nonzero constant term makes both of these poles genuine.

We first justify the initial [Mellin transform](../../../../../mellin-transform.md). Decompose $f=a_0E_k+h$ with $h\in S_k$. For a [cusp form](../../../../../cusp-form.md), $y^{k/2}|h(x+iy)|$ is invariant under the [modular group](../../../../../modular-group.md) and bounded on its fundamental domain, since it tends to zero at the cusp. Therefore it is bounded throughout the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Integrating the [Fourier coefficient](../../../../../fourier-coefficient.md) at height $y=1/n$ gives $|a_n(h)|\leq Ce^{2\pi}n^{k/2}$. The [Eisenstein series](../../../../../eisenstein-series.md) coefficients satisfy $\sigma_{k-1}(n)\leq\zeta(k-1)n^{k-1}$ by replacing divisors $d$ by $n/d$. Consequently $a_n(f)=O(n^{k-1})$, and absolute termwise integration is valid for $\Re s>k$:

$$
\Lambda_f(s)=\int_0^\infty(f(iy)-a_0)y^{s-1}\,dy.
$$

Indeed $\int_0^\infty e^{-2\pi ny}y^{s-1}\,dy=(2\pi n)^{-s}\Gamma(s)$, and the sum of the absolute integrals converges in that half-plane.

Write $I_f(s)=\int_1^\infty(f(iy)-a_0)y^{s-1}\,dy$. Exponential cusp decay of the difference implies uniform convergence on compact subsets of the $s$-plane, including after any number of derivatives in $s$, so $I_f$ is entire. The modular transformation $f(i/y)=(iy)^kf(iy)$ gives

$$
f(iy)=\varepsilon y^{-k}f(i/y).
$$

On the lower half of the Mellin integral, subtract the transformed constant explicitly:

$$
f(iy)-a_0=\varepsilon y^{-k}(f(i/y)-a_0)+a_0(\varepsilon y^{-k}-1).
$$

Substitute $y=1/t$ in the decaying term and integrate the two powers in the constant term. This yields, initially for $\Re s>k$,

$$
\boxed{\Lambda_f(s)=I_f(s)+\varepsilon I_f(k-s)+a_0\left(\frac{\varepsilon}{s-k}-\frac1s\right).}
$$

The right side supplies the claimed [meromorphic continuation](../../../../../meromorphic-continuation.md) and its residues. Replacing $s$ by $k-s$ and multiplying by $\varepsilon$, with $\varepsilon^2=1$, leaves this expression unchanged, proving the [functional equation](../../../../../functional-equation.md) with its correct sign. In particular the residue at $k$ is tied to the residue at zero by that equation; subtracting only $a_0$ at infinity and overlooking its transformed value at zero would miss these poles.

In weight zero every [modular form](../../../../../modular-form.md) is constant, so $L(f,s)=0$ and its completion is identically zero. The same holds for the zero form in odd, negative, or weight-two spaces. Thus the assertion covers all weights in the notation of the paper. There is no conjugation of $f$ in this level-one functional equation.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
