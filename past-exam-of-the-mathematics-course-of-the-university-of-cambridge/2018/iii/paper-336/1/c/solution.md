<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The ordinary [saddle-point approximation with a nearby pole](../../../../../../saddle-point-approximation-with-a-nearby-pole.md) loses uniformity when the pole lies within the width of the saddle's [Gaussian function](../../../../../../gaussian-function.md) profile. The [distinguished limit](../../../../../../distinguished-limit.md) is

$$
\boxed{z_d=z_s=i,\qquad z_0-i=O(k^{-1/2}).}
$$

Use the exact quadratic phase coordinate $s=2i\sqrt{k}(u-1)$ and define

$$
\boxed{s_d=2i\sqrt{k}\bigl(e^{-i\pi/4}\sqrt{z_0}-1\bigr)
=\sqrt{k}(z_0-i)+O\bigl(\sqrt{k}(z_0-i)^2\bigr).}
$$

On the descending contour, $s$ runs along the real axis from $-\infty$ to $+\infty$. The transformed differential has the useful [partial fraction decomposition](../../../../../../partial-fraction-decomposition.md)

$$
\frac{dz}{z-z_0}=\left(\frac1{u-u_0}+\frac1{u+u_0}\right)du,
\qquad u_0=e^{-i\pi/4}\sqrt{z_0}.
$$

The first term contains the nearby pole; the second is regular at the saddle and contributes $O(e^{-k}k^{-1/2})$. Approaching from below the descending contour means $\operatorname{Im}s_d<0$. The [residue theorem](../../../../../../residue-theorem.md) then gives the [Gaussian saddle-pole transition](../../../../../../gaussian-saddle-pole-transition.md)

$$
J(z_0)=e^{-k}\left[\int_{-\infty}^{\infty}\frac{e^{-s^2/4}}{s-s_d}\,ds+2\pi i e^{-s_d^2/4}\right]+O(e^{-k}k^{-1/2}).
$$

The exponent is $-s^2/4$, as in the original PDF; the converted TeX's $-s^2/2$ is a transcription error. The exact identity $k\phi(z_0)=-k-s_d^2/4$ recovers the pole exponential in the requested expression.

The [Gaussian pole integral](../../../../../../gaussian-pole-integral.md) expresses the bracket as $i\pi w(s_d/2)$, where $w$ is the [Faddeeva function](../../../../../../faddeeva-function.md). Thus a convenient uniform leading answer is

$$
\boxed{J(z_0)=i\pi e^{-k}w(s_d/2)+O(e^{-k}k^{-1/2}).}
$$

The error estimate applies for bounded scaled pole position on the indicated side. In the overlap $1\ll|s_d|\ll\sqrt{k}$ below the real axis, the integral contributes $-2\sqrt\pi/s_d$ to leading order while the residue remains $2\pi i e^{-s_d^2/4}$. Since $s_d\sim\sqrt{k}(z_0-i)$, this reproduces the near-saddle limit of the separate saddle and residue terms. Boundary values on the descending contour are limits of this combined expression; the isolated real-axis pole integral itself needs a [Cauchy principal value](../../../../../../cauchy-principal-value.md) prescription.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
