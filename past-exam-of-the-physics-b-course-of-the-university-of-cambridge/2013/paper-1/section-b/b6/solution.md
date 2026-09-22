<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

The [image charge](../../../../../image-charge.md) construction replaces conductor-induced charge by fictitious sources outside the physical domain. Match the conductor potentials and the far-field condition; uniqueness then fixes the potential in the physical region. For a grounded plane, reflect a charge and reverse its sign, giving attraction $q^2/(16\pi\epsilon_0h^2)$. For a grounded sphere of radius $a$, a charge at distance $R>a$ has image $-qa/R$ at radial distance $a^2/R$. These are examples with prescribed zero potential, not arbitrary isolated conductors.[grounded plane construction and its uniqueness argument](../../../../../method-of-images-by-richard-fitzpatrick.md)

Use horizontal $x$ and upward $y$ in the upper right-angle wedge. The sheets meet electrically, so take their common potential as zero and assume no externally imposed field. For a real charge at $(0,y)$, the [image charges in a right-angle conducting wedge](../../../../../image-charges-in-a-right-angle-conducting-wedge.md) are $-q$ at $(y,0)$ and $(-y,0)$, and $+q$ at $(0,-y)$. The first two contributions have cancelling horizontal components. With $K_e=1/(4\pi\epsilon_0)$,

$$
F_y=-\frac{K_eq^2}{\sqrt2y^2}+\frac{K_eq^2}{4y^2}
=-\frac\beta{y^2},\qquad
\boxed{\beta=\frac{q^2(2\sqrt2-1)}{16\pi\epsilon_0}.}
$$

Thus the [force](../../../../../force-split.md) magnitude at the original height is $\beta/y_0^2$, directed down toward the intersection. The sphere is treated as a [point charge](../../../../../point-charge.md), with size much smaller than its distances from the sheets.

Since gravity is already balanced in the uncharged [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), the charged vertical [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) satisfies $k(y_e-y_0)+\beta/y_e^2=0$. For $\beta/(ky_0^3)\ll1$, $y_e\simeq y_0-\beta/(ky_0^2)$. Differentiating the [force](../../../../../force-split.md) gives

$$
\omega_y^2=\frac1m\left(k-\frac{2\beta}{y_e^3}\right),\qquad
\boxed{\frac{\omega_y-\omega_0}{\omega_0}\simeq-\frac{\beta}{ky_0^3},\quad\omega_0=\sqrt{k/m}.}
$$

The [electrostatic softening above a conducting wedge](../../../../../electrostatic-softening-above-a-conducting-wedge.md) reduces the restoring [force](../../../../../force-split.md); the small-charge vertical [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) remains stable.

For the [lateral stability of a spring-supported charge in a wedge](../../../../../lateral-stability-of-a-spring-supported-charge-in-a-wedge.md), the off-axis images of $(x,y)$ are $-q$ at $(y,x)$ and $(-y,-x)$ and $+q$ at $(-x,-y)$. Expansion near the bisector gives

$$
F_x=D_xx+O(x^3),\qquad
D_x=\frac{K_eq^2}{y_e^3}\left(\sqrt2+\frac14\right)>0.
$$

So **the electrostatic [force](../../../../../force-split.md) is laterally destabilizing**: moving toward either sheet strengthens its attraction. In the simplified model where the [spring](../../../../../spring.md) supplies only a vertical [force](../../../../../force-split.md), the overall [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is a saddle and is unstable.

A three-dimensional [spring](../../../../../spring.md) suspension also has geometrical transverse stiffness. If its charged-equilibrium tension is $T$ and [length](../../../../../length.md) is $\ell$, a small sideways displacement gives [spring](../../../../../spring.md) [force](../../../../../force-split.md) $-(T/\ell)x$, with $T=mg+\beta/y_e^2$. The full stability conditions in this suspension model are

$$
\boxed{k>\frac{2\beta}{y_e^3},\qquad\frac T\ell>D_x.}
$$

Motion parallel to the intersection line has no electrostatic stiffness in the ideal infinite-wedge geometry and is stabilized by the positive [spring](../../../../../spring.md) tension. Thus **lateral electrostatic destabilization alone does not prove instability of a real hanging spring**. At fixed finite support geometry, a sufficiently small charge preserves stability because $D_x=O(q^2)$ while $T/\ell\to mg/\ell>0$. The given vertical-displacement approximation does not specify the attachment [length](../../../../../length.md) or by itself establish the transverse inequality for an arbitrary charge. The general criterion above states what can be concluded; the saddle verdict applies to the distinct idealization with zero lateral support stiffness.

<a id="section-b/b6/image-original-image-charge-field-construction-and-the-opposite-signs-of-vertical-softening-and-lateral-electrostatic-stiffness"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-1-image-wedge.png)

**[Figure 1](#section-b/b6/image-original-image-charge-field-construction-and-the-opposite-signs-of-vertical-softening-and-lateral-electrostatic-stiffness). Original image-charge field construction and the opposite signs of vertical softening and lateral electrostatic stiffness**.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
