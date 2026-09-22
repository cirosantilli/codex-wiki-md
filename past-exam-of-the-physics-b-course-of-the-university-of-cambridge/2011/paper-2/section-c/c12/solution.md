<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

Write $\mu=GM$ and $A=\mu m$. For a [circular orbit](../../../../../circular-orbit.md) of radius $r$, centripetal balance gives $v^2=\mu/r$. Thus $E=mv^2/2-A/r=-A/(2r)$ and $J^2=m^2r^2v^2=Amr$. Since $e=0$, $a=r_0=r$, these agree with the general expressions.

For an outward coplanar [Hohmann transfer](../../../../../hohmann-transfer-orbit.md), burn prograde at the inner [circle](../../../../../circle.md) to put its radius at the ellipse's [pericentre](../../../../../periapsis.md), then burn prograde at [apocentre](../../../../../apoapsis.md) to circularize at the station's radius. The station must be phased to meet the spacecraft there. With $r_p=R$, $r_a=\alpha R$,

$$
\boxed{a_T=\frac{1+\alpha}{2}R,\qquad e_T=\frac{\alpha-1}{\alpha+1},\qquad r_0=a_T(1-e_T^2)=\frac{2\alpha R}{1+\alpha}.}
$$

[Energy](../../../../../energy-split.md) at the first burn, with $v_0^2=\mu/R$, gives

$$
\frac{v_1^2}{2}-\frac\mu R=-\frac\mu{(1+\alpha)R},\qquad
\boxed{v_1=v_0\sqrt{\frac{2\alpha}{1+\alpha}}.}
$$

[Angular momentum](../../../../../angular-momentum.md) is conserved along the transfer ellipse, so $v_{2-}=v_1/\alpha$, while the outer circular speed is $v_{2+}=v_0/\sqrt\alpha$. For $\alpha=3$,

$$
\boxed{v_{2-}=\frac{v_0}{\sqrt6},\qquad v_{2+}=\frac{v_0}{\sqrt3}.}
$$

The correct second [impulse](../../../../../impulse.md) adds $\Delta v=v_{2+}-v_{2-}$. The [reversed circularization burn in a Hohmann transfer](../../../../../reversed-circularization-burn-in-a-hohmann-transfer.md), using the _same_ [impulse](../../../../../impulse.md) magnitude, instead leaves

$$
v_w=2v_{2-}-v_{2+}=v_0\left(\frac2{\sqrt6}-\frac1{\sqrt3}\right)>0.
$$

Its magnitude is below the circular speed at $3R$, so that point is the new [apocentre](../../../../../apoapsis.md). Define $q=r_a v_w^2/\mu=(\sqrt2-1)^2=3-2\sqrt2$. For an ellipse at [apocentre](../../../../../apoapsis.md), $q=1-e_w$, giving

$$
\boxed{e_w=2\sqrt2-2\simeq0.8284,\qquad
r_{p,w}=3R\frac{1-e_w}{1+e_w}=3R\frac{3-2\sqrt2}{2\sqrt2-1}\simeq0.2815R.}
$$

The lunar radius is $R/3$. Since $r_{p,w}<R/3$, **the osculating [orbit](../../../../../orbit-dynamical-system.md) intersects the [Moon](../../../../../moon.md): the spacecraft crashes before reaching its formal [pericentre](../../../../../periapsis.md).** The calculation uses impulsive tangential burns and a spherical central gravitational field; it does not assume that a trajectory continues through the solid body.

<a id="section-c/c12/image-correct-and-reversed-transfer-burn"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2-transfer-orbits.png)

**[Figure 2](#section-c/c12/image-correct-and-reversed-transfer-burn). Correct and reversed transfer burn**.

The original plot uses $R$ as the length unit and $R/3$ as the lunar radius. The initial station position shown is phased for rendezvous: its initial angular lead is $\pi-\pi[(1+\alpha)/(2\alpha)]^{3/2}$, modulo $2\pi$.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
