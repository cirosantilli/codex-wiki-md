<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Gaussian pole transition for a large gamma parameter](../../../../../../gaussian-pole-transition-for-a-large-gamma-parameter.md). With $t=1+s/\sqrt n$ and $\lambda=n+i\mu\sqrt n+\nu+o(1)$, [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
(n-1)\log t+\lambda(1-t)
=-\frac{s^2}{2}-i\mu s+\frac1{\sqrt n}\left(\frac{s^3}{3}-(1+\nu)s\right)+O(n^{-1}(1+|s|^4)),
\qquad \frac{dt}{1-t}=-\frac{ds}{s}.
$$

The upper semicircle is traversed from left to right, so $\int ds/s=-i\pi$ on the indentation. The minus sign in $dt/(1-t)$ therefore makes its contribution $+i\pi$. The remaining leading integral is

$$
I_0(\mu)=i\pi-\operatorname{PV}\int_{-\infty}^{\infty}\frac{e^{-s^2/2-i\mu s}}s\,ds.
$$

At $\mu=0$ its [Cauchy principal value](../../../../../../cauchy-principal-value.md) vanishes by oddness. Differentiating with respect to $\mu$ removes the [pole](../../../../../../pole.md), leaving the [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md):

$$
I_0'(\mu)=i\sqrt{2\pi}e^{-\mu^2/2}.
$$

Integrating from zero gives

$$
\boxed{I(\lambda,n)=i\pi\left[1+\operatorname{erf}\left(\frac\mu{\sqrt2}\right)\right]+O(n^{-1/2})}.
$$

This is uniform for bounded real $\mu,\nu$ (and extends analytically over bounded complex values where the local contour is continued consistently). Contributions away from the saddle are exponentially small after localization. The bounded shift $\nu$ enters at the next order, not the leading [error function](../../../../../../error-function.md). For example, retaining the displayed cubic correction gives $\sqrt{2\pi/n}e^{-\mu^2/2}[\nu+(2+\mu^2)/3]$ as the next term. This also checks the constant and contour sign.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
