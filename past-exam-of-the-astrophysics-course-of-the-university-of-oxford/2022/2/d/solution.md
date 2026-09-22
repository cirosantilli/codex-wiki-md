<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a regular spherical star, let $\rho_c=\rho(0)$ and $P_c=P(0)$. The [stellar mass conservation equation](../../../../stellar-mass-conservation-equation.md) and [stellar hydrostatic equation](../../../../hydrostatic-pressure-support-equation.md) are

$$
M'(r)=4\pi r^2\rho(r),\qquad P'(r)=-\frac{GM(r)\rho(r)}{r^2}.
$$

Assuming the smoothness needed for the requested [Taylor series](../../../../taylor-series.md), write $M=a_0+a_1r+a_2r^2+a_3r^3+\cdots$. There is no point [mass](../../../../mass.md) at the centre, so $a_0=0$, and matching the [stellar mass conservation equation](../../../../stellar-mass-conservation-equation.md) gives $a_1=a_2=0$, $a_3=4\pi\rho_c/3$. Substitution in the [stellar hydrostatic equation](../../../../hydrostatic-pressure-support-equation.md) gives $P'(r)=-(4\pi G/3)\rho_c^2r+O(r^3)$, hence

$$
\boxed{M(r)=\frac{4\pi}{3}\rho_cr^3+O(r^5),\qquad
P(r)=P_c-\frac{2\pi G}{3}\rho_c^2r^2+O(r^4).}
$$

The remainder orders use a smooth spherically symmetric scalar [density](../../../../density.md), for which $\rho(r)=\rho_c+O(r^2)$. Merely finite continuous [density](../../../../density.md) gives the same leading coefficients with $o(r^3)$ and $o(r^2)$ remainders. In particular $P'(0)=0$, despite the apparent $r^{-2}$ in the [stellar hydrostatic equation](../../../../hydrostatic-pressure-support-equation.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
