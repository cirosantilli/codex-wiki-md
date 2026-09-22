<h1 id="section-b/b3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In [Newtonian gravity](../../../../../gravitational-acceleration.md), the radial equation with conserved [specific angular momentum](../../../../../specific-angular-momentum.md) is $\ddot r=-GM/r^2+h^2/r^3$. The substitution $u=1/r$ therefore gives the linear [differential equation](../../../../../differential-equation-split.md)

$$
u''+u=\frac{GM}{h^2}.
$$

Choosing $\phi=0$ along perihelion, its [elliptic orbit](../../../../../elliptic-orbit.md) solution is

$$
\boxed{u_0(\phi)=\frac{1+e\cos\phi}{p},\qquad
p=\frac{h^2}{GM}=a_{\rm orb}(1-e^2).}
$$

Here $p$ is the [semilatus rectum](../../../../../semilatus-rectum.md). One can check the last equality directly from $r_{\rm peri}=p/(1+e)$, $r_{\rm apo}=p/(1-e)$, and $a_{\rm orb}=(r_{\rm peri}+r_{\rm apo})/2$.

To find [Schwarzschild perihelion precession](../../../../../schwarzschild-perihelion-precession.md), write $u=u_0+\delta u$ in the relativistic equation and retain first order in $\mu/p$. The [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) for the correction is

$$
\delta u''+\delta u=3\mu u_0^2
=\frac{3\mu}{p^2}\left(1+\frac{e^2}{2}+2e\cos\phi+\frac{e^2}{2}\cos2\phi\right).
$$

The constant and double-frequency forcing change the orbit's shape without accumulating an angular shift. The resonant $\cos\phi$ term produces

$$
\delta u_{\rm sec}=\frac{3\mu e}{p^2}\,\phi\sin\phi,
$$

since $(d^2/d\phi^2+1)(\phi\sin\phi)=2\cos\phi$. The oscillating part of the perturbed orbit is consequently the first-order expansion of

$$
\frac e p\cos\big[(1-3\mu/p)\phi\big].
$$

Successive perihelia are separated by $2\pi/(1-3\mu/p)$, slightly more than a full revolution. Their forward angular advance is thus

$$
\boxed{\Delta\phi=\frac{6\pi\mu}{p}
=\frac{6\pi GM}{c^2a_{\rm orb}(1-e^2)}
+O\!\left(\frac{\mu^2}{p^2}\right)}
$$

in radians per orbit. This leading expression applies when $\mu/p\ll1$. For a perfectly [circular orbit](../../../../../circular-orbit.md) there is no uniquely located perihelion; the same expression describes the limiting mismatch of radial and azimuthal frequencies for a small nonzero [orbital eccentricity](../../../../../orbital-eccentricity.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B3](../../b3.md)
3. [Section B](../../../section-b.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the relativity course of the University of Cambridge](../../../../split.md)
6. [Relativity course of the University of Cambridge](../../../../../relativity-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
