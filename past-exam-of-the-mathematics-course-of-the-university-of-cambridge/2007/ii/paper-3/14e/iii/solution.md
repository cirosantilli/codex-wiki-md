<h1 id="14e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With $\sigma=1$, substitute $x=(u+v)/2$, $y=(u-v)/2$, $r=1+\mu$. The equations become

$$
\boxed{\dot u=\tfrac12(\mu-z)(u+v),\quad
\dot v=-2v-\tfrac12(\mu-z)(u+v),\quad
\dot z=\tfrac14(u^2-v^2)-bz,\quad\dot\mu=0.}
$$

The extended centre variables are $u,\mu$. The [centre manifold theorem](../../../../../../centre-manifold-theorem.md) gives smooth graph functions $V,Z$ with $V(0,0)=Z(0,0)=0$ and all first derivatives zero. Their invariance equations are $V_u\dot u=\dot v$ and $Z_u\dot u=\dot z$, after substitution of the graph.

Count $\mu$ as order $u^2$. Then $\dot u=O(u^3)$ on the graph, so the left side of the $Z$ equation contributes only at higher order. Its quadratic terms give $0=u^2/4-bZ$, hence $Z=u^2/(4b)+O(u^3)$. The cubic terms of the $V$ equation similarly give $0=-2V-\mu u/2+uZ/2$. Thus

$$
\boxed{Z=\frac{u^2}{4b}+O(u^3),\qquad
V=-\frac{\mu u}{4}+\frac{u^3}{16b}+O(u^4).}
$$

Terms purely in $\mu$ vanish because the origin remains an [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) for every parameter; these expansions describe the weighted scaling $\mu=O(u^2)$, not an unrestricted one-variable Taylor [series](../../../../../../series-mathematics.md). Substitution gives the reduced equation

$$
\boxed{\dot u=\frac\mu2u-\frac1{8b}u^3+O(u^4).}
$$

Its cubic coefficient is negative. For $\mu<0$ the origin is attracting in the centre direction; for $\mu>0$ it loses stability and two attracting branches emerge with $u\sim\pm2\sqrt{b\mu}$. Therefore the bifurcation is a **supercritical pitchfork**. These branches agree with the exact Lorenz equilibria $x=y=\pm\sqrt{b\mu}$, $z=\mu$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [14E](../../14e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
