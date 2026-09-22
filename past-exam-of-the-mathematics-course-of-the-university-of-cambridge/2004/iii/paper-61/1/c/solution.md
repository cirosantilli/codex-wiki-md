<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the negative-exponential [Half-range Fourier transform](../../../../../../half-range-fourier-transform.md)

$$
\widehat q(k,t)=\int_0^\infty e^{-ikx}q(x,t)\,dx,\qquad F(k)=\widehat q(k,0),\qquad \operatorname{Im}k\leq0.
$$

For the boundary traces $g_j(t)=\partial_x^jq(0,t)$, define [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md) $G_j(k,t)=\int_0^t e^{w(k)s}g_j(s)\,ds$. Integrating the conservation law in $x$ and then time gives the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md)

$$
e^{w(k)t}\widehat q(k,t)=F(k)+G_2(k,t)+ikG_1(k,t)-(k^2+1)G_0(k,t).
$$

The plus sign of the boundary contribution follows because the integrated flux is $-E(0,t)X(0,t,k)$.

[Fourier inversion](../../../../../../fourier-inversion-theorem.md) consequently gives a real-line initial integral plus a boundary integral. To put the latter in the complex plane, define

$$
D_+=\{k=u+iv:v>0,\ \operatorname{Re}w(k)<0\}=\{u+iv:v>\sqrt{3u^2+1}\}.
$$

Orient $\partial D_+$ from the left upper infinity, through $i$, to the right upper infinity, with $D_+$ on the left. Each $G_j$ is entire, and in the region between the real axis and this contour, $\operatorname{Re}w\geq0$. The causal factors $e^{-w(t-s)}$ are bounded there and $e^{ikx}$ decays for $x>0$. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md), with the usual large-arc limiting argument, deforms the boundary integral to give

$$
\boxed{q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-wt}F(k)\,dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-wt}\bigl[G_2+ikG_1-(k^2+1)G_0\bigr]dk.}
$$

Initial smoothness, spatial decay and corner compatibility justify inversion; if necessary the integrals are first regularized before contour deformation. The unknown Neumann-type traces $g_1,g_2$ will be removed by the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
