<h1 id="9b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [inferring an inverse-square force from Kepler laws](../../../../../../inferring-an-inverse-square-force-from-kepler-laws.md), first use the area swept by an infinitesimal radius sector:

$$
\dot{\mathcal A}=\frac12r^2\dot\theta.
$$

[Kepler's second law](../../../../../../kepler-s-second-law.md) makes the [areal velocity](../../../../../../areal-velocity.md) constant, so $l=r^2\dot\theta$ is constant. Then $r\ddot\theta+2\dot r\dot\theta=0$, meaning that the acceleration has no transverse component. [Newton's second law](../../../../../../newton-s-second-law.md) therefore gives a [central force](../../../../../../central-force.md) directed along the Sun–planet line.

For the radial dependence, set $u=1/r$. Since $\dot\theta=lu^2$,

$$
\dot r=-l u_\theta,\qquad
\ddot r=-l^2u^2u_{\theta\theta},\qquad
r\dot\theta^2=l^2u^3.
$$

The radial acceleration is the [Binet equation](../../../../../../binet-equation.md) expression

$$
a_r=-l^2u^2(u_{\theta\theta}+u).
$$

The focus-based [ellipse](../../../../../../ellipse.md) has $u=(1+\varepsilon\cos\theta)/A$, hence $u_{\theta\theta}+u=1/A$. Thus

$$
\boxed{a_r=-\frac{l^2}{A r^2}.}
$$

For a planet of mass $m$, the [force](../../../../../../force.md) is $F_r=-ml^2/(Ar^2)$: it is attractive and obeys the [inverse-square law](../../../../../../inverse-square-law.md). This deduction uses both the shape of the orbit and its constant [areal velocity](../../../../../../areal-velocity.md); the orbit shape alone would not determine its time-dependent acceleration.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9B](../../9b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
