<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $|\zeta|=1$ and $|z|<1$, the [Poisson kernel on the circle](../../../../../poisson-kernel-on-the-circle.md) satisfies

$$
\operatorname{Re}\frac{\zeta+z}{\zeta-z}
=\frac{1-|z|^2}{|\zeta-z|^2}\geq0.
$$

For fixed $\zeta$, it is the real part of a [holomorphic function](../../../../../holomorphic-function.md) of $z$, hence a [harmonic function](../../../../../harmonic-function.md). On each compact subdisk, its derivatives are bounded uniformly in $\zeta$ because the denominator stays away from zero. Differentiation under the integral therefore proves that $P\phi$ is [harmonic](../../../../../harmonic-function.md), with the word interpreted componentwise when $\phi$ is complex-valued.

The [geometric series](../../../../../geometric-series.md)

$$
\frac{\zeta+z}{\zeta-z}=1+2\sum_{n\geq1}z^n\zeta^{-n}
$$

converges uniformly in $\zeta$ for a fixed compact subdisk. With normalized [Lebesgue measure](../../../../../lebesgue-measure.md), integration of its real part gives kernel mass one. Fix a boundary point $\omega$ and choose $\delta>0$ so that $|\phi(\zeta)-\phi(\omega)|<\varepsilon$ when $|\zeta-\omega|<\delta$. Then

$$
|P\phi(z)-\phi(\omega)|
\leq\varepsilon+2\|\phi\|_\infty
\int_{|\zeta-\omega|\geq\delta}\frac{1-|z|^2}{|\zeta-z|^2}\,dm(\zeta).
$$

If $z\to\omega$ from inside the [unit disc](../../../../../unit-disc.md), the remaining denominator is at least $(\delta/2)^2$ for sufficiently close $z$, while $1-|z|^2\to0$. Hence **$P\phi(z)\to\phi(\omega)$ along every interior approach**, not just radial ones.

Orient the unit circle counterclockwise in the [Cauchy transform](../../../../../cauchy-transform.md). Its kernel and every $w$-derivative are uniformly bounded for $w$ in any compact subset of $\mathbb C\setminus\mathbb T$. Thus differentiation under the integral gives

$$
\Phi'(w)=\frac1{2\pi i}\int_{\mathbb T}\frac{\phi(\zeta)}{(\zeta-w)^2}\,d\zeta,
$$

and proves that $\Phi$ is a [holomorphic function](../../../../../holomorphic-function.md) on both components of its domain. Since $d\zeta=2\pi i\zeta\,dm(\zeta)$, for $0<r<1$ and $|\omega|=1$ the difference of its two kernels is

$$
\frac{\zeta}{\zeta-r\omega}-\frac{\zeta}{\zeta-r^{-1}\omega}
=\frac{1-r^2}{|\zeta-r\omega|^2}.
$$

Consequently the [paired radial jump of a continuous Cauchy transform](../../../../../paired-radial-jump-of-a-continuous-cauchy-transform.md) obeys the exact identity

$$
\boxed{\Phi(r\omega)-\Phi(r^{-1}\omega)=P\phi(r\omega)\quad(0<r<1)},
$$

and the established [Poisson integral](../../../../../poisson-integral.md) boundary convergence gives

$$
\boxed{\Phi(r\omega)-\Phi(r^{-1}\omega)\longrightarrow\phi(\omega)
\quad\text{as }r\uparrow1.}
$$

This proves the paired difference without assuming that the two individual boundary values exist for every continuous datum.

**The printed direction $r\downarrow1$ has the opposite sign.** It is present in the original PDF, not merely in the converted TeX. With that direction $r>1$, so substituting $s=1/r<1$ in the exact identity gives

$$
\boxed{\Phi(r\omega)-\Phi(r^{-1}\omega)=-P\phi(r^{-1}\omega)\longrightarrow-\phi(\omega).}
$$

The simplest counterexample is $\phi\equiv1$: the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) gives $\Phi(w)=1$ inside and $\Phi(w)=0$ outside, so the printed difference is constantly $-1$. The requested positive jump is corrected by taking $r\uparrow1$, or by reversing the order of the difference when $r\downarrow1$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
