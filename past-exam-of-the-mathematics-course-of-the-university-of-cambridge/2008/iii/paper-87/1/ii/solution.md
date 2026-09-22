<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $F(r)=r^4u^3K(r)$ and retain the scalar trace correlation $C(r)$. For radial functions the [Laplacian](../../../../../../laplacian.md) is $\nabla^2C=r^{-2}(r^2C')'$. Multiplying the trace [Kármán-Howarth equation](../../../../../../karman-howarth-equation.md) by the radial volume element and integrating gives

$$
\dot L=4\pi\left[\frac{F'}r\right]_0^\infty
+8\pi\nu[r^2C']_0^\infty.
$$

Regularity at the origin removes the lower endpoints. The stated triple-correlation tail gives $F=u^3(a+b/r+\cdots)$ and hence $F'/r\to0$. Rapid enough decay of the trace correlation removes the viscous endpoint. Therefore

$$
\boxed{\dot L=0.}
$$

For the [Loitsyansky integral](../../../../../../loitsyansky-integral.md), multiplying by $-4\pi r^4$ gives the nonlinear contribution

$$
\dot I_{\rm nl}=-4\pi\int_0^\infty r^2\left(\frac{F'}r\right)'dr
=-4\pi[rF']_0^\infty+8\pi[F]_0^\infty
=8\pi F(\infty).
$$

The given tail removes $rF'$ but permits a nonzero limit of $F$. The viscous contribution is

$$
\begin{aligned}
\dot I_\nu
&=-8\pi\nu\int_0^\infty r^2(r^2C')'dr\\
&=-8\pi\nu[r^4C']_0^\infty+16\pi\nu[r^3C]_0^\infty
-48\pi\nu\int_0^\infty r^2C(r)dr\\
&=-12\nu L.
\end{aligned}
$$

Here the stronger weighted endpoints vanish under the assumed sufficiently rapid correlation decay. Combining the terms yields

$$
\boxed{\frac{dI}{dt}=8\pi[r^4u^3K]_\infty-12\nu L.}
$$

The conserved [Saffman integral](../../../../../../saffman-integral.md) measures the density of large-volume [momentum](../../../../../../momentum.md) fluctuations established in part (i). Internal interactions redistribute [momentum](../../../../../../momentum.md) without changing that leading extensive [variance](../../../../../../variance-split.md) when forcing and far-field [momentum](../../../../../../momentum.md) fluxes are absent. This is a statistical expression of [linear momentum](../../../../../../momentum.md) conservation, not the assertion that kinetic energy is conserved during viscous decay.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
