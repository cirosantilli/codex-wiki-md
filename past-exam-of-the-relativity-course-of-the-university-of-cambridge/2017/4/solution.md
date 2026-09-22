<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Curvature contractions.** Use the index contraction stipulated in the question. In three dimensions,

$$
R_{jk}=g^{il}K(g_{ik}g_{jl}-g_{il}g_{jk})=K(g_{jk}-3g_{jk})=-2Kg_{jk}.
$$

The same contraction in four dimensions gives

$$
R_{\beta\gamma}=-\frac\Lambda3(g_{\beta\gamma}-4g_{\beta\gamma})=\Lambda g_{\beta\gamma}.
$$

Then the [Ricci scalar](../../../ricci-scalar.md) is $R=4\Lambda$ and the [Einstein tensor](../../../einstein-tensor.md) is $G_{\mu\nu}=-\Lambda g_{\mu\nu}$. Thus $R_{\mu\nu}=\Lambda g_{\mu\nu}$ is precisely the vacuum [Einstein field equations](../../../einstein-field-equations-split.md) $G_{\mu\nu}+\Lambda g_{\mu\nu}=0$.

**The static solution.** For $A=1+\lambda^2r^2$, $A'=2\lambda^2r$ and $A''=2\lambda^2$. The given [Ricci tensor](../../../ricci-tensor.md) components become

$$
R_{00}=-3\lambda^2A,\quad R_{11}=\frac{3\lambda^2}{A},\quad
R_{22}=3\lambda^2r^2,\quad R_{33}=3\lambda^2r^2\sin^2\theta.
$$

Each equals $-3\lambda^2$ times the corresponding [metric tensor](../../../metric-tensor.md) component. Therefore

$$
\boxed{\Lambda=-3\lambda^2.}
$$

This is [Anti-de Sitter spacetime](../../../anti-de-sitter-spacetime.md) in [static coordinates on anti-de Sitter spacetime](../../../static-coordinates-on-anti-de-sitter-spacetime.md), with curvature radius $1/\lambda$. The overall [metric signature](../../../metric-signature.md) is opposite to the convention used in some descriptions of those coordinates; the geodesic constants below use the question's $(+,-,-,-)$ convention.

**Conserved quantities and radial motion.** In the equatorial plane, the [geodesic Lagrangian](../../../geodesic-lagrangian.md) is $L=A\dot t^2-\dot r^2/A-r^2\dot\phi^2$. Its [cyclic coordinates](../../../cyclic-coordinate.md) give

$$
\boxed{k=A\dot t,\qquad h=r^2\dot\phi.}
$$

For rest [mass](../../../mass.md) $m$, $mk=p_t$ is the conserved Killing [energy](../../../energy-split.md) and $mh=-p_\phi$ is the axial [angular momentum](../../../angular-momentum.md). Timelike normalization $L=1$ gives

$$
\boxed{\dot r^2=k^2-A\left(1+\frac{h^2}{r^2}\right)
=k^2-1-\lambda^2h^2-\lambda^2r^2-\frac{h^2}{r^2}.}
$$

For purely radial motion $h=0$, differentiating away from a turning point gives $\ddot r=-\lambda^2r$, and continuity extends that equation through the turning point. An outward launch from the origin at $\tau=0$ has

$$
\boxed{r(\tau)=\frac{\sqrt{k^2-1}}\lambda\sin(\lambda\tau),\qquad
a=\frac{\sqrt{k^2-1}}\lambda,\quad b=\lambda.}
$$

This is the [radial timelike geodesic in anti-de Sitter spacetime](../../../radial-timelike-geodesic-in-anti-de-sitter-spacetime.md). Its first return to the origin is

$$
\boxed{\tau_{\rm return}=\frac\pi\lambda,}
$$

independent of the outward launch speed for every nontrivial launch $k>1$. The coordinate $r$ is nonnegative, so this sine expression describes the excursion up to that return; subsequent passage through the origin requires changing the radial direction or using a signed diameter coordinate. The speed changes the amplitude, not the harmonic frequency.

**Circular periods.** The effective radial potential is $V_{\rm eff}=A(1+h^2/r^2)$. For a circle at $r_0$, $V_{\rm eff}'=0$ gives $h^2=\lambda^2r_0^4$, and normalization gives $k=A(r_0)$. Thus $\dot t=1$ and $\dot\phi=\pm\lambda$. A [stable circular timelike geodesic in anti-de Sitter spacetime](../../../stable-circular-timelike-geodesic-in-anti-de-sitter-spacetime.md) therefore has

$$
\boxed{\Delta t=\Delta\tau=\frac{2\pi}\lambda,}
$$

independently of radius. This is the same isochronous behavior as the central harmonic radial equation. A static clock placed at the orbit's radius instead measures $\sqrt{1+\lambda^2r_0^2}\,\Delta t$, which does depend on radius; it is a different clock from the orbiting particle's [proper time](../../../proper-time.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2017](../../2017-split.md)
3. [Past exam of the relativity course of the University of Cambridge](../../split.md)
4. [Relativity course of the University of Cambridge](../../../relativity-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
