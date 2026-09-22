<h1 id="section-d/d17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**[Separation of variables](../../../../../../separation-of-variables.md) replaces a compatible [partial differential equation](../../../../../../partial-differential-equation-split.md) by ordinary differential [eigenvalue](../../../../../../eigenvalue.md) equations.** For example, with a thermally diffusive rod, $u_t=D u_{xx}$, try $u=X(x)T(t)$. Wherever division is valid,

$$
\frac{T'}{DT}=\frac{X''}{X}=-\lambda.
$$

The two sides depend on independent variables, so each must be constant. Homogeneous end temperatures $u(0,t)=u(L,t)=0$ give $X_n=\sin(n\pi x/L)$ and $\lambda_n=(n\pi/L)^2$. The general initial-temperature profile is represented by superposing these separated modes:

$$
\boxed{u(x,t)=\sum_{n=1}^\infty b_n\sin\frac{n\pi x}{L}\,e^{-D(n\pi/L)^2t},\qquad
b_n=\frac2L\int_0^L u(x,0)\sin\frac{n\pi x}{L}\,dx.}
$$

Each spatial mode decays at its own rate. For a fixed-end [wave equation](../../../../../../wave-equation-split.md) the same spatial [eigenfunctions](../../../../../../eigenfunction.md) instead have oscillatory time factors $A_n\cos(cn\pi t/L)+B_n\sin(cn\pi t/L)$, with coefficients fixed by initial [displacement](../../../../../../displacement.md) and velocity. Similar constructions separate [Laplace's equation](../../../../../../laplace-equation.md) in suitable coordinate systems.

A single product is usually only one mode, not the most general solution. Linear [superposition](../../../../../../superposition-principle.md) and [completeness](../../../../../../completeness.md) of the spatial [eigenfunctions](../../../../../../eigenfunction.md) are what extend the method to general allowed data. Nonhomogeneous boundary values can first be removed by a known stationary or particular solution. Separation is effective when the geometry, coefficients and [boundary conditions](../../../../../../boundary-condition.md) admit a common separated eigenproblem; an arbitrary nonlinear equation or inseparable geometry need not do so. Self-adjoint [Sturm-Liouville problems](../../../../../../sturm-liouville-problem.md) explain the weighted [orthogonality](../../../../../../orthogonal-vectors.md) and [completeness](../../../../../../completeness.md) in many physical applications.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D17](../../d17.md)
3. [Section D](../../../section-d.md)
4. [Paper 2A](../../../../paper-2a-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
