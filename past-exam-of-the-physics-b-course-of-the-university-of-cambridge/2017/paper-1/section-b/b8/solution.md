<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

**Field law and centre value.** The [Biot-Savart law](../../../../../biot-savart-law.md) for a steady thin wire is

$$
d\mathbf B=\frac{\mu_0I}{4\pi}
\frac{d\boldsymbol\ell'\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}.
$$

Here $d\boldsymbol\ell'$ follows the conventional [electric current](../../../../../electric-current.md) and the displacement points from source to observation point. For a circular loop of radius $a$, every element at the centre has distance $a$ and contributes in the same axial direction. Choose $+z$ by the [right-hand rule](../../../../../right-hand-rule.md). Then

$$
\boxed{\mathbf B(0)=\frac{\mu_0I}{4\pi a^2}(2\pi a)\widehat{\mathbf z}
=\frac{\mu_0I}{2a}\widehat{\mathbf z}.}
$$

**On-axis integration.** At axial distance $z$, every wire element has distance $\sqrt{a^2+z^2}$. Azimuthal symmetry cancels transverse components. Parameterizing $\mathbf r'=(a\cos\varphi,a\sin\varphi,0)$ gives axial cross-product element $a^2\,d\varphi$, so the [on-axis magnetic field of a circular current loop](../../../../../on-axis-magnetic-field-of-a-circular-current-loop.md) is

$$
\boxed{\mathbf B(0,z)=B_0(z)\widehat{\mathbf z},\qquad
B_0(z)=\frac{\mu_0Ia^2}{2(a^2+z^2)^{3/2}}.}
$$

It points the same way on the two halves of the axis; its strength is even in $z$.

**Directions near the axial point.** At a point on the positive axis the field is axial, but nearby lines spread outward because $B_0$ decreases as $z$ increases. On the negative-axis side they converge toward the axis while still progressing in the positive axial direction. There is no azimuthal field. The near-axis sketch shows this local spreading; the complete [magnetic field lines](../../../../../magnetic-field-line.md) return around the outside of the loop and form closed curves.

<a id="section-b/b8/image-original-calculated-leading-near-axis-field-line-geometry-on-the-positive-side-of-a-circular-current-loop-the-lines-spread-as-the-axial-field-weakens"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1-b8-near-axis-loop-field.png)

**[Figure 2](#section-b/b8/image-original-calculated-leading-near-axis-field-line-geometry-on-the-positive-side-of-a-circular-current-loop-the-lines-spread-as-the-axial-field-weakens). Original calculated leading near-axis field-line geometry on the positive side of a circular current loop; the lines spread as the axial field weakens**.

**Radial component from zero divergence.** Smooth axial symmetry gives $B_z(\rho,z)=B_0(z)+O(\rho^2)$ and $B_\rho=O(\rho)$. By [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md),

$$
\frac1\rho\partial_\rho(\rho B_\rho)+\partial_zB_z=0.
$$

Integrate radially from zero, excluding a singular $1/\rho$ term, to obtain the [near-axis radial magnetic field](../../../../../near-axis-radial-magnetic-field.md), $B_\rho=-\rho B_0'(z)/2+O(\rho^3)$. Differentiating the axial field therefore gives

$$
\boxed{B_\rho\simeq
\frac{3\mu_0Ia^2z\rho}{4(a^2+z^2)^{5/2}}.}
$$

For $z>0$ it is outward; for $z<0$ it is inward. This supplies the direction reasoning used in the sketch.

**Force on the second loop.** Put the second loop at $z=d$ and radius $\rho=a$. For $d\gg a$, the radial field due to the first loop is $B_\rho\simeq3\mu_0Ia^3/(4d^4)$. The element $d\boldsymbol\ell=a\,d\varphi\,\widehat{\boldsymbol\varphi}$ experiences [Lorentz force](../../../../../lorentz-force.md)

$$
d\mathbf F=I a\,d\varphi\left(B_z\widehat{\boldsymbol\rho}-B_\rho\widehat{\mathbf z}\right).
$$

The radial contributions cancel as vectors around the loop. The axial contributions add, giving the [force between distant coaxial current loops](../../../../../force-between-distant-coaxial-current-loops.md),

$$
\boxed{F_z=-2\pi aI B_\rho
\simeq-\frac{3\pi\mu_0I^2a^4}{2d^4}.}
$$

The sign follows $\widehat{\boldsymbol\varphi}\times\widehat{\boldsymbol\rho}=-\widehat{\mathbf z}$. Both the small radial coordinate relative to $d$ and the dipole approximation are justified by $a/d\ll1$.

**Force direction.** The second loop is pulled back toward the first: **the force is attractive** for the same current sense. Reversing one current reverses the [force](../../../../../force-split.md). The much larger axial field chiefly produces radial element forces; retaining the smaller radial field is essential for the net axial attraction.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
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
