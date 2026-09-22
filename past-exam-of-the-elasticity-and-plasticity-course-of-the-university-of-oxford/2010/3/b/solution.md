<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Contract the [tensors](../../../../tensor.md), counting both off-diagonal shear terms:

$$
\mathcal W=\frac12\tau_{ij}e_{ij}
=\frac{Ez^2}{2(1-\nu^2)}
\{a^2+2\nu ac+c^2+2(1-\nu)b^2\}.
$$

Since $\int_{-h/2}^{h/2}z^2\,dz=h^3/12$, integration gives

$$
\boxed{\int_{-h/2}^{h/2}\mathcal W\,dz
=\frac D2\{a^2+2\nu ac+c^2+2(1-\nu)b^2\},\qquad
D=\frac{Eh^3}{12(1-\nu^2)}.}
$$

For the general midplane deflection, expand the energy [density](../../../../density.md) as $w_{xx}^2+2\nu w_{xx}w_{yy}+w_{yy}^2+2(1-\nu)w_{xy}^2$. A variation $w+\varepsilon\eta$ gives

$$
\delta\mathcal U=D\iint_\Omega
\{(w_{xx}+\nu w_{yy})\eta_{xx}
+(w_{yy}+\nu w_{xx})\eta_{yy}+2(1-\nu)w_{xy}\eta_{xy}\}\,dx\,dy.
$$

For clamped variations, $\eta=\partial_n\eta=0$ on the boundary, so integrating twice transfers all derivatives to $w$ without a boundary contribution. The bulk coefficient is

$$
w_{xxxx}+2\nu w_{xxyy}+w_{yyyy}+2(1-\nu)w_{xxyy}
=(\partial_x^2+\partial_y^2)^2w.
$$

Stationarity for all compactly supported variations and the fundamental lemma therefore give

$$
\boxed{\nabla^4w=0\quad\text{in the plate interior}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
