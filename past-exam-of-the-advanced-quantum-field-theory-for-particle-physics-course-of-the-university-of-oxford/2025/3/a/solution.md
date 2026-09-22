<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start with the formally gauge-redundant [path integral](../../../../path-integral.md) $Z=\operatorname{vol}(\mathcal G)^{-1}\int\mathcal DA\,e^{iS[A]}$. Use $A_\mu^\theta=A_\mu+\partial_\mu\theta$, and the generalized [Lorenz gauge condition](../../../../lorenz-gauge-condition.md) $F_\omega[A]=\partial_\mu A^\mu-\omega$. In a perturbative neighborhood where residual zero modes are removed by [boundary conditions](../../../../boundary-condition.md), insert the [Faddeev-Popov gauge-orbit identity](../../../../faddeev-popov-gauge-orbit-identity.md)

$$
1=\Delta_{\rm FP}[A]\int\mathcal D\theta\,
\delta[F_\omega(A^\theta)],\qquad
\frac{\delta F_\omega(A^\theta)(x)}{\delta\theta(y)}
=\Box_x\delta^{(4)}(x-y).
$$

Thus $\Delta_{\rm FP}=\det\Box$. [Gauge invariance](../../../../gauge-invariance.md) lets the $\theta$ integration factor out and cancel $\operatorname{vol}(\mathcal G)$. Average over $\omega$ with the [Gaussian integral](../../../../gaussian-integral.md) weight $\exp[-i\int\omega^2/(2\xi)]$; the delta functional fixes $\omega=\partial\cdot A$ and gives

$$
\mathcal L_{\rm gf}=-\frac1{2\xi}(\partial\cdot A)^2.
$$

Represent the [functional determinant](../../../../functional-determinant.md) by the independent [Grassmann fields](../../../../grassmann-field.md) $\bar c,c$. A field-independent determinant sign can be absorbed in normalization, so a convenient convention is

$$
\det\Box\ \propto\ \int\mathcal D\bar c\mathcal Dc\,
\exp\left[-i\int d^4x\,\bar c\Box c\right].
$$

Therefore

$$
\boxed{Z=\mathcal N\int\mathcal DA\mathcal D\bar c\mathcal Dc\,
\exp\left\{i\int d^4x\left[-\frac14F_{\mu\nu}F^{\mu\nu}
-\frac1{2\xi}(\partial\cdot A)^2-\bar c\Box c\right]\right\}.}
$$

The [Faddeev-Popov ghosts](../../../../faddeev-popov-ghost.md) are free and decouple because $\Box$ is independent of $A$. For a [Non-Abelian gauge theory](../../../../yang-mills-theory.md), an infinitesimal [gauge transformation](../../../../gauge-transformation.md) gives $\delta A_\mu^a=D_\mu^{ab}\theta^b$, so the [Faddeev-Popov operator](../../../../faddeev-popov-operator.md) is $\partial^\mu D_\mu^{ab}[A]$ and

$$
\mathcal L_{\rm gh}=-\bar c^a\partial^\mu D_\mu^{ab}[A]c^b.
$$

It contains a [ghost-gluon vertex](../../../../ghost-gluon-vertex.md): these [Faddeev-Popov ghosts](../../../../faddeev-popov-ghost.md) do not decouple in covariant [gauge fixing](../../../../gauge-fixing.md) of [Lorenz gauge](../../../../lorenz-gauge-condition.md) type.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
