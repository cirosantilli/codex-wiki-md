<h1 id="k/k2/solution">Solution</h1>

↑ **Parent:** [K2](../k2.md)

Orient the body boundary $C$ counterclockwise. Its outward [normal vector](../../../../normal-vector.md) satisfies $\mathbf n\,ds=(dy,-dx)$, so the [pressure](../../../../pressure-split.md) force on the body has complex component

$$
F_x-iF_y=-i\oint_C p\,d\bar z.
$$

For steady [incompressible flow](../../../../incompressible-flow.md) and [irrotational flow](../../../../irrotational-flow.md), [Bernoulli's principle](../../../../bernoulli-s-principle.md) gives $p=p_0-\rho|w'|^2/2$. The constant-[pressure](../../../../pressure-split.md) integral vanishes. Write $q=w'=u-iv$. The [impermeability condition](../../../../no-penetration-boundary-condition.md) makes velocity tangent to $C$, implying $q\,dz=\bar q\,d\bar z$. Thus $|q|^2d\bar z=q^2dz$ along the boundary, and

$$
\boxed{F_x-iF_y=\frac{i\rho}{2}\oint_C(w')^2\,dz}.
$$

This proves the [Blasius force theorem](../../../../blasius-force-theorem.md), with force measured per unit length perpendicular to the flow plane.

For a circle of radius $a$, [Milne-Thomson's circle theorem](../../../../milne-thomson-circle-theorem.md) replaces an incident analytic potential $f(z)$ by $f(z)+\overline{f(a^2/\bar z)}$, making the [stream function](../../../../stream-function.md) constant on the circle. Its reflected singularities must lie inside the circle; here the physical source lies outside. With $c=Q/(2\pi)$ and $d=a^2/b$, this yields, up to additive constants,

$$
w(z)=c\bigl[\log(z-b)+\log(z-d)-\log z\bigr],\qquad
w'=c\left(\frac1{z-b}+\frac1{z-d}-\frac1z\right).
$$

The interior image source and sink have equal and opposite strengths, so there is no extra net source inside the body. No independent vortex term is added. The potential may have logarithmic branches, but the velocity and [pressure](../../../../pressure-split.md) are single-valued.

Only $d$ and $0$ lie inside $C$. The residues of $(w')^2$ are

$$
\operatorname{Res}_d(w')^2=2c^2\left(\frac1{d-b}-\frac1d\right),\qquad
\operatorname{Res}_0(w')^2=2c^2\left(\frac1b+\frac1d\right).
$$

Their sum is $-2c^2a^2/[b(b^2-a^2)]$. The [residue theorem](../../../../residue-theorem.md) and the preceding force formula therefore give

$$
\boxed{F_x=\frac{\rho Q^2a^2}{2\pi b(b^2-a^2)},\qquad F_y=0}.
$$

The force points towards the external source. [Reflection](../../../../reflection-mathematics.md) symmetry across the horizontal axis independently checks the vanishing vertical component.

## ↑ Ancestors (12)

1. [K2](../k2.md)
2. [K](../../k.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
