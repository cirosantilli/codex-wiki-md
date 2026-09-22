<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First remove the observation time from the spectral amplitude. For any fixed horizon $H>t$, replace $G_0(k,t)$ by $G_0(k,H)$ in the formula of part (d). The difference in the boundary integral is proportional to

$$
\int_{\partial D_+}e^{ikx}(3k^2+1)\int_t^H e^{w(k)(s-t)}g_0(s)\,ds\,dk.
$$

For every $s>t$, this integrand is holomorphic inside $D_+$, where $\operatorname{Re}w<0$, and decays on its large closing arcs. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) makes the difference zero. This [finite-horizon extension of a boundary transform](../../../../../../finite-horizon-extension-of-a-boundary-transform.md) therefore gives the time-independent spectra

$$
F(k),\qquad \mathcal B_H(k)=\mathcal TF(k)+(3k^2+1)\int_0^H e^{w(k)s}g_0(s)\,ds.
$$

All observation-time dependence is now in $e^{ikx-wt}$.

When the boundary history is sufficiently decaying, the natural long-time version is

$$
\boxed{\mathcal B_\infty(k)=\mathcal TF(k)+(3k^2+1)\int_0^\infty e^{w(k)s}g_0(s)\,ds.}
$$

The integral converges in $\operatorname{Re}w<0$ for bounded boundary data and on its boundary for integrable histories; otherwise one must state an Abel prescription or a suitable temporal growth assumption. Arbitrary smooth $g_0$ need not have such an infinite-time transform. The finite-horizon formula remains exact without that extra assumption, and the source alone does not prescribe a universal long-time limit.

A useful further decomposition, if $g_0(s)=g_\infty+r(s)$ with integrable $r$, is

$$
\int_0^\infty e^{ws}g_0(s)ds=-\frac{g_\infty}{w}+R(w),\qquad R(w)=\int_0^\infty e^{ws}r(s)ds,\qquad \operatorname{Re}w<0.
$$

This separates the persistent forcing from the transient spectrum. The pole at $k=i$, where $w=0$, accounts for the decaying stationary profile $g_\infty e^{-x}$; that profile also follows directly from $q_{xxx}-q_x=0$, spatial decay and its boundary value. For the remaining oscillatory integrals the phase is $i[kx+(k^3+k)t]$. At a fixed ray $x/t=\xi$, its stationary points satisfy $3k^2+1+\xi=0$, or $k=\pm i\sqrt{(1+\xi)/3}$. These time-independent amplitudes expose precisely the poles and saddle points used in the [method of steepest descent](../../../../../../method-of-steepest-descent.md); allowable deformations must also respect the analyticity strip of the initial transform.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
