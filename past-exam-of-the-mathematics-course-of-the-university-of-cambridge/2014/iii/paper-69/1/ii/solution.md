<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [Fourier inversion](../../../../../../fourier-inversion-theorem.md) to the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) on the real axis, extending $u$ by zero to negative $x$. At an interior point $x>0$ this gives

$$
u(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega t}\widehat u_0(k)\,dk
-\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega t}[G_1+(ik+\alpha)G_0](k,t)\,dk.
$$

The [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md) are [entire functions](../../../../../../entire-function.md) of $k$. Define the upper decay domain

$$
D^+=\{k=a+ib:b>0,\ \operatorname{Re}\omega(k)<0\}
=\{a+ib:b>\alpha,\ a^2<b(b-\alpha)\}.
$$

Orient $\partial D^+$ from its left infinite end through $i\alpha$ to its right infinite end, so that $D^+$ lies to the left. Its finite point is $i\alpha$, not zero. On the contour, $\operatorname{Re}\omega=0$; the factor $e^{ikx}$ decays because $x>0$.

For the boundary term, write $e^{-\omega t}G_j=\int_0^t e^{-\omega(t-s)}g_j(s)\,ds$. Between the real axis and $\partial D^+$, $\operatorname{Re}\omega\geq0$, so this factor has no exponential growth. [Contour deformation](../../../../../../contour-deformation.md) and [Jordan lemma](../../../../../../jordan-s-lemma.md), with the usual cutoffs for oscillatory integrals, therefore give

$$
\boxed{u(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega t}\widehat u_0(k)\,dk
-\frac1{2\pi}\int_{\partial D^+}e^{ikx-\omega t}[G_1+(ik+\alpha)G_0](k,t)\,dk.}
$$

This is the requested complex-plane representation with the unknown [finite-time spectral boundary transform](../../../../../../finite-time-spectral-boundary-transform.md) still present. The decay domain must agree with the sign of the drift in the [dispersion relation](../../../../../../dispersion-relation.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
