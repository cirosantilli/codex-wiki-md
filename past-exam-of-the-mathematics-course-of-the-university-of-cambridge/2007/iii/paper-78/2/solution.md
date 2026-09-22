<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [slender viscous bubble](../../../../../slender-viscous-bubble.md), approximate the interface normal by the radial direction and its curvature by $1/a$. Axial curvature and axial derivatives of the leading external motion are smaller by the slenderness factors. The exterior leading [Stokes flow](../../../../../stokes-flow-split.md) is locally radial. Incompressibility gives $\partial_r(ru_r)=0$, while the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) gives $u_r(a)=a_t$ to leading order, hence

$$
u_r(r,z,t)=\frac{a(z,t)a_t(z,t)}r.
$$

The radial viscous Laplacian of this $1/r$ [velocity](../../../../../velocity.md) vanishes, so exterior [pressure](../../../../../pressure.md) is constant to leading order; set its reference value to zero. Its radial [normal stress](../../../../../normal-stress.md) at the interface is $2\mu\partial_ru_r|_a=-2\mu a_t/a$. Inner viscous [normal stress](../../../../../normal-stress.md) is smaller by the viscosity ratio $\lambda$, and the bubble's leading [normal stress](../../../../../normal-stress.md) is $-P$. The [interfacial stress balance with variable surface tension](../../../../../interfacial-stress-balance-with-variable-surface-tension.md), here with constant $\gamma$, consequently gives

$$
P-\frac{2\mu a_t}a=\frac\gamma a,\qquad\boxed{P=\frac{2\mu a_t}a+\frac\gamma a.}
$$

These are local leading-order relations: the outer axial flow and tangential traction enter at higher slenderness order. The sign also has a useful check: a uniform cylinder with no imposed excess [pressure](../../../../../pressure.md) contracts, $a_t=-\gamma/(2\mu)$, under [surface tension](../../../../../surface-tension.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
