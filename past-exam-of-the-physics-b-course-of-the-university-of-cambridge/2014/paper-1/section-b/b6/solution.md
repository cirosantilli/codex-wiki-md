<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Specifying potential on the complete boundary gives a [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) and a unique harmonic solution. Specifying its normal derivative gives a [Neumann boundary condition](../../../../../neumann-boundary-condition.md), with the zero-net-flux compatibility condition and an undetermined additive constant. Mixed conditions on complementary portions also give uniqueness when a potential reference is fixed. In an exterior domain, conditions at infinity are needed. These statements follow by applying [Green's first identity](../../../../../green-s-first-identity.md) to the difference of two solutions. A metal in [electrostatic equilibrium](../../../../../electrostatic-equilibrium.md) is an equipotential: $\Phi=V_0$, tangential [electric field](../../../../../electric-field-split.md) zero, and normal field $E_n=\sigma/\epsilon_0$ just outside a vacuum interface.

For the [conducting-wedge potential expansion](../../../../../conducting-wedge-potential-expansion.md), put $u=\Phi-V_0$ in the empty sector $0<\theta<\alpha$. For $u=r^\nu\Psi(\theta)$, Laplace's equation gives $\Psi''+\nu^2\Psi=0$. Vanishing values on both faces require $\Psi\propto\sin(n\pi\theta/\alpha)$, hence

$$
\boxed{\Phi=V_0+\sum_{n=1}^{\infty}\left(a_nr^{n\pi/\alpha}+b_nr^{-n\pi/\alpha}\right)\sin\frac{n\pi\theta}{\alpha}.}
$$

Bounded potential at the corner sets $b_n=0$. The coefficients still require outer boundary data; the metal potential alone cannot select them. For a generic nonzero $a_1$, put $p=\pi/\alpha$. Differentiation gives

$$
\boxed{E_r\simeq-pa_1r^{p-1}\sin p\theta,\qquad E_\theta\simeq-pa_1r^{p-1}\cos p\theta.}
$$

If $a_1=0$, the first nonzero higher harmonic replaces this leading term. For $\alpha=\pi/2$, $u\simeq2a_1xy$, so $\mathbf E=-2a_1(y,x)$ and field lines satisfy **$x^2-y^2=\mathrm{constant}$**, meeting the metal faces normally and tending to zero field at the corner. For $\alpha=3\pi/2$, the [electrostatic corner-field exponent](../../../../../electrostatic-corner-field-exponent.md) is $-1/3$. A real tip's rounding cuts off this divergence; breakdown or [field emission](../../../../../field-electron-emission.md) can limit the attainable field.

<a id="section-b/b6/image-original-right-angle-field-line-calculation-and-the-two-corner-field-power-laws"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-1-wedge-field.png)

**[Figure 1](#section-b/b6/image-original-right-angle-field-line-calculation-and-the-two-corner-field-power-laws). Original right-angle field-line calculation and the two corner-field power laws**.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
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
