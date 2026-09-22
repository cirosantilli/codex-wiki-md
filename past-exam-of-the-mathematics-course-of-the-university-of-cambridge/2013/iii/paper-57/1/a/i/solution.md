<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the dimensionless [quantum phase](../../../../../../../quantum-phase.md) $S$, so that $\psi=R e^{iS}$ with $R\geq0$. Work locally away from [wavefunction](../../../../../../../wave-function.md) nodes, where $R$ and $S$ are differentiable. Differentiating the [wavefunction](../../../../../../../wave-function.md) for substitution in the [Time-dependent Schrödinger equation](../../../../../../../time-dependent-schrodinger-equation.md) gives:

$$
\partial_t\psi=e^{iS}(R_t+iRS_t),\qquad
\nabla^2\psi=e^{iS}\left[\nabla^2R-R|\nabla S|^2+i(2\nabla R\cdot\nabla S+R\nabla^2S)\right].
$$

Cancel $e^{iS}$ in the time-dependent equation and equate real and imaginary parts. The resulting [Madelung equations](../../../../../../../madelung-equations.md) are

$$
\boxed{R_t=-\frac{\hbar}{2m}\left(2\nabla R\cdot\nabla S+R\nabla^2S\right)},\qquad
\boxed{\hbar S_t+\frac{\hbar^2}{2m}|\nabla S|^2+V-\frac{\hbar^2}{2m}\frac{\nabla^2R}{R}=0}.
$$

The second equation is a [Hamilton-Jacobi equation](../../../../../../../hamilton-jacobi-equation.md) for the action $\hbar S$, with an additional [quantum potential](../../../../../../../quantum-potential.md). To see the meaning of the first, multiply it by $2R$ and set $\rho=R^2$. It becomes the [probability continuity equation](../../../../../../../probability-continuity-equation.md)

$$
\partial_t\rho+\nabla\cdot\left(\rho\frac{\hbar}{m}\nabla S\right)=0.
$$

Thus the [probability density](../../../../../../../probability-density.md) is transported by the velocity field $\hbar\nabla S/m$. The [Madelung equations](../../../../../../../madelung-equations.md) are a local rewriting of the linear wave equation; their apparent nonlinearity comes from expressing a complex [wavefunction](../../../../../../../wave-function.md) in modulus and phase variables.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
