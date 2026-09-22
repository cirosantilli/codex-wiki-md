<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

**Definition and equations.** A [normal mode](../../../../../normal-mode.md) is a motion in which every component of a [linear system](../../../../../system-of-linear-equations.md) has the same time dependence with fixed amplitude ratios and phases. For a conservative system near equilibrium, the most useful form is

$$
\mathbf q(t)=\operatorname{Re}\{a\,\mathbf u\,e^{-i\omega t}\}.
$$

The [vector](../../../../../vector.md) $\mathbf u$ describes the [mode shape](../../../../../mode-shape.md), while $\omega$ is its [angular frequency](../../../../../angular-frequency.md). Linear combinations of modes describe arbitrary sufficiently small motions when the modes form a complete [basis](../../../../../basis.md).

Let $q_i$ be displacements of independent [generalized coordinates](../../../../../generalized-coordinate.md) from equilibrium. Expand the [Lagrangian](../../../../../lagrangian.md) to quadratic order:

$$
L=\frac12\dot{\mathbf q}^{\mathsf T}M\dot{\mathbf q}
-\frac12\mathbf q^{\mathsf T}K\mathbf q,
\qquad M\ddot{\mathbf q}+K\mathbf q=0.
$$

The [mass matrix](../../../../../mass-matrix.md) $M$ defines a [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md) on the independent coordinates, while the [stiffness matrix](../../../../../stiffness-matrix.md) $K$ is the [Hessian](../../../../../hessian-matrix.md) of the [potential energy](../../../../../potential-energy.md). Substituting a mode gives the [generalized eigenvalue problem for small oscillations](../../../../../generalized-eigenvalue-problem-for-small-oscillations.md)

$$
\boxed{K\mathbf u=\omega^2M\mathbf u,
\qquad \det(K-\omega^2M)=0.}
$$

A practical calculation identifies the equilibrium, chooses independent coordinates, computes the quadratic kinetic and potential [energies](../../../../../energy-split.md), solves for the [eigenvalues](../../../../../eigenvalue.md) and then obtains their [eigenvectors](../../../../../eigenvector.md). One can equivalently diagonalize the real symmetric [matrix](../../../../../matrix.md) $M^{-1/2}KM^{-1/2}$. This guarantees real $\omega^2$ and a complete [orthogonal basis](../../../../../orthogonal-basis.md) in mass-weighted coordinates.

For distinct [eigenvalues](../../../../../eigenvalue.md), the fact that $K$ and $M$ are real [symmetric matrices](../../../../../symmetric-matrix.md) implies

$$
(\omega_i^2-\omega_j^2)\mathbf u_j^{\mathsf T}M\mathbf u_i=0.
$$

Thus distinct modes are [orthogonal](../../../../../orthogonal-vectors.md) in the [inner product](../../../../../inner-product-split.md) weighted by the [mass matrix](../../../../../mass-matrix.md). Choosing $\mathbf u_i^{\mathsf T}M\mathbf u_j=\delta_{ij}$ decouples the motion into $\ddot Q_i+\omega_i^2Q_i=0$, with total [energy](../../../../../energy-split.md) $\sum_i(\dot Q_i^2+\omega_i^2Q_i^2)/2$. A [positive-definite matrix](../../../../../positive-definite-matrix.md) $K$ gives positive [eigenvalues](../../../../../eigenvalue.md) and oscillatory stability. Zero modes can describe rigid translations or [rotations](../../../../../rotation-mathematics.md) without restoring [force](../../../../../force-split.md); a negative [eigenvalue](../../../../../eigenvalue.md) gives exponential instability rather than an oscillatory mode.

**[Symmetry](../../../../../symmetry-physics.md).** A [symmetry](../../../../../symmetry-physics.md) preserving both quadratic [energies](../../../../../energy-split.md) maps modes into modes of the same [frequency](../../../../../frequency.md). Coordinates adapted to [symmetry](../../../../../symmetry-physics.md) divide the [eigenvalue](../../../../../eigenvalue.md) problem into smaller independent blocks. For two identical subsystems, exchanging them gives symmetric and antisymmetric modes. The [degeneracy of normal modes](../../../../../degeneracy-of-normal-modes.md) means that independent modes share one [frequency](../../../../../frequency.md). Higher-dimensional [group representations](../../../../../group-representation.md) of a [symmetry](../../../../../symmetry-physics.md) can enforce such degeneracies; [symmetry](../../../../../symmetry-physics.md) does not require every pair of modes to be degenerate, and accidental degeneracies can also occur. Within a degenerate [eigenspace](../../../../../eigenspace.md), [orthogonal](../../../../../orthogonal-vectors.md) linear combinations are equally valid [mode shapes](../../../../../mode-shape.md).

For two equal masses $m$, each attached to a fixed support by a spring of stiffness $k$ and coupled to the other by a spring of stiffness $k_c$,

$$
K=\begin{pmatrix}k+k_c&-k_c\\-k_c&k+k_c\end{pmatrix},\qquad M=m\mathsf I.
$$

The symmetric mode $\mathbf u_+\propto(1,1)$ leaves the coupling spring unstretched and has $\omega_+^2=k/m$. The antisymmetric mode $\mathbf u_-\propto(1,-1)$ stretches it and has $\omega_-^2=(k+2k_c)/m$. Superposing the two gives [beats](../../../../../beat.md) when their [frequencies](../../../../../frequency.md) are close.

**Continuous systems.** The same idea replaces matrices by [differential operators](../../../../../differential-operator.md) and mode [vectors](../../../../../vector.md) by functions satisfying [boundary conditions](../../../../../boundary-condition.md). For a taut string of length $L$, [tension](../../../../../tension.md) $\mathcal T$ and [mass](../../../../../mass.md) per unit length $\mu_\ell$, the [wave equation](../../../../../wave-equation-split.md) and fixed endpoints give

$$
y_n(x,t)=A_n\sin(n\pi x/L)\cos(\omega_nt+\phi_n),
\qquad \omega_n=\frac{n\pi}{L}\sqrt{\frac{\mathcal T}{\mu_\ell}},\quad n\geq1.
$$

[Orthogonality](../../../../../orthogonal-vectors.md) of the [sine](../../../../../sine.md) functions allows an arbitrary initial [displacement](../../../../../displacement.md) to be decomposed into modes. Changing the endpoints changes the spectrum: [boundary conditions](../../../../../boundary-condition.md) are part of the physical mode problem.

A uniform chain of equal masses $m$ joined by springs $k_s$, with spacing $a$, has travelling [normal modes](../../../../../normal-mode.md) $q_j\propto e^{i(kja-\omega t)}$ with

$$
\omega^2(k)=\frac{4k_s}{m}\sin^2(ka/2).
$$

Their quantization gives [phonons](../../../../../phonon.md); the long-wavelength limit is a [sound](../../../../../soundness.md) wave. [Rectangular electromagnetic cavity](../../../../../rectangular-electromagnetic-cavity.md) modes satisfy [Maxwell's equations](../../../../../maxwell-equations-split.md) and conductor [boundary conditions](../../../../../boundary-condition.md), with $\omega=c|\mathbf k|$ in [vacuum](../../../../../vacuum.md). An [elastic beam](../../../../../elastic-beam.md) instead has a fourth-order spatial equation and flexural dispersion $\omega\propto k^2$. These examples show how restoring [forces](../../../../../force-split.md) and geometry determine the [frequency spectrum](../../../../../frequency-spectrum.md).

**Real systems.** Small-amplitude motion is often approximately linear even when the full equations are nonlinear. Large amplitudes produce [frequency](../../../../../frequency.md) shifts, mode coupling and transfer of [energy](../../../../../energy-split.md) between modes. Friction broadens resonances and makes free oscillations decay. A [damping](../../../../../damping.md) [matrix](../../../../../matrix.md) proportional to $M$ or $K$ can retain the undamped [mode shapes](../../../../../mode-shape.md); general [damping](../../../../../damping.md) need not, and the appropriate eigenfrequencies and modes can be complex. External periodic forcing predominantly excites modes near [resonance](../../../../../resonance.md), with amplitude set by coupling to the forcing and dissipation. Imperfections split ideal degeneracies, while radiation or coupling to a surrounding fluid can remove [energy](../../../../../energy-split.md) from the chosen subsystem. **[Normal modes](../../../../../normal-mode.md) remain useful when [linearization](../../../../../linearization.md), the [boundary conditions](../../../../../boundary-condition.md) and the treatment of [damping](../../../../../damping.md) accurately describe the motion being measured.**

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
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
