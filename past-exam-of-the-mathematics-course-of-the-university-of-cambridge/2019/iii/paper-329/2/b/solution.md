<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each broad face supplies [surface tension](../../../../../../surface-tension.md) $\gamma$ pulling the rounded hole edge into the remaining sheet. Their resultant is $2\gamma$ per unit circumference. At the inner boundary the fluid's outward normal is $-\mathbf e_r$, so the boundary [traction](../../../../../../traction.md) is outward in the radial direction when $h\sigma_{rr}=-2\gamma$. The right panel of the preceding diagram shows these two capillary pulls.

With uniform thickness and $p_{\rm ext}=0$, the [axisymmetric viscous-sheet stretching equations](../../../../../../axisymmetric-viscous-sheet-stretching-equations.md) reduce to

$$
r u_{rr}+u_r-u/r=0.
$$

This [Euler-Cauchy equation](../../../../../../euler-cauchy-equation.md) gives $u=Ar+B/r$. The fixed outer rim imposes $u(R_0)=0$, hence $B=-AR_0^2$. Because $(ru)_r/r=2A$, [conservation of mass](../../../../../../mass-conservation.md) gives $\dot h=-2Ah$, independent of $r$. Thus a uniform sheet remains uniform.

The radial [stress](../../../../../../stress.md) is $\sigma_{rr}=6\mu A-2\mu B/r^2$. Its value at the hole edge determines

$$
\boxed{A=-\frac{\gamma R^2}{\mu h(R_0^2+3R^2)},\qquad
B=\frac{\gamma R^2R_0^2}{\mu h(R_0^2+3R^2)}.}
$$

The edge is material, so $\dot R=u(R)$ and

$$
\dot R=\frac{\gamma R(R_0^2-R^2)}{\mu h(R_0^2+3R^2)}.
$$

Neglecting the initially tiny hole's volume, [conservation of mass](../../../../../../mass-conservation.md) gives $\pi h(R_0^2-R^2)=\pi h_0R_0^2$, or $h=h_0/(1-x^2)$ with $x=R/R_0$. Therefore the [capillary growth of a hole in a viscous sheet](../../../../../../capillary-growth-of-a-hole-in-a-viscous-sheet.md) obeys

$$
\boxed{\frac{dx}{dt}=\frac{\gamma}{\mu h_0}\frac{x(1-x^2)^2}{1+3x^2}.}
$$

For a finite initial hole $x_i$, replace $h_0$ in the denominator by $h_0(1-x_i^2)$. A nonzero seed is needed: the exact initial condition $x(0)=0$ gives the stationary solution of this differential equation. For a small positive seed, $x$ initially grows exponentially at rate $\gamma/(\mu h_0)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
