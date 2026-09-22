<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the negative-exponential [Half-range Fourier transforms](../../../../../../half-range-fourier-transform.md)

$$
\widehat q_0(k)=\int_0^\infty e^{-ikx}q_0(x)\,dx,
\qquad\widehat q(k,t)=\int_0^\infty e^{-ikx}q(x,t)\,dx,
$$

which are [holomorphic](../../../../../../complex-differentiability-at-a-point.md) for $\operatorname{Im}k<0$. Write $g_j(s)=\partial_x^jq(0,s)$ and define the [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md)

$$
G_j(k,t)=\int_0^t e^{\omega(k)s}g_j(s)\,ds\qquad(j=0,1,2).
$$

Integrate the [local relation](../../../../../../local-relation.md) over $0<x<\infty$, $0<s<t$. The spatial boundary term at infinity vanishes by decay, and the term at $x=0$ is subtracted. Consequently the [half-line linear dispersive Stokes global relation](../../../../../../half-line-linear-dispersive-stokes-global-relation.md) is

$$
\boxed{e^{\omega(k)t}\widehat q(k,t)=\widehat q_0(k)+B(k,t),\qquad
B=(1-k^2)G_0+ikG_1+G_2,\quad\operatorname{Im}k\leq0.}
$$

[Fourier inversion](../../../../../../fourier-inversion-theorem.md) on the real axis gives an initial-data [integral](../../../../../../integral.md) plus an [integral](../../../../../../integral.md) of $B$. To put the boundary term on a complex [contour](../../../../../../complex-integration-contour.md), set

$$
D_+=\{k:\operatorname{Im}k>0,\ \operatorname{Re}\omega(k)<0\}.
$$

For $k=u+iv$, $\operatorname{Re}\omega=v(3u^2-v^2-1)$, so $D_+$ is the connected upper domain $v>0$, $v^2>3u^2-1$. Orient $\partial D_+$ with this domain on the left: from upper-left infinity down to $-1/\sqrt3$, along the real segment to $1/\sqrt3$, and then to upper-right infinity.

The [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md) are [entire functions](../../../../../../entire-function.md). In the upper regions outside $D_+$, where $\operatorname{Re}\omega\geq0$, their time-integrated factors satisfy $|e^{-\omega t}e^{\omega s}|\leq1$ for $0\leq s\leq t$. Together with $e^{ikx}$, this permits [contour deformation](../../../../../../contour-deformation.md) of the two remaining real-axis pieces to the curved boundary of $D_+$. The resulting representation is

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega(k)t}\widehat q_0(k)\,dk
+\frac1{2\pi}\int_{\partial D_+}e^{ikx-\omega(k)t}\bigl[(1-k^2)G_0+ikG_1+G_2\bigr]dk.}
$$

The [contour](../../../../../../complex-integration-contour.md) orientation accounts for the plus sign in this convention. This formula still contains the two unknown derivative traces through $G_1,G_2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
