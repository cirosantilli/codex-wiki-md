<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let a [gauge transformation](../../../../../../gauge-transformation.md) act infinitesimally as $\delta A_\mu^a=(D_\mu\omega)^a$, and define the [Faddeev-Popov operator](../../../../../../faddeev-popov-operator.md) by variation of the chosen gauge functional:

$$
\mathcal M^{ab}[A](x,y)=\left.\frac{\delta\mathcal F^a[A^\omega](x)}{\delta\omega^b(y)}\right|_{\omega=0}.
$$

Work in a perturbative [regular gauge slice](../../../../../../regular-gauge-slice.md), with boundary conditions that remove residual zero modes and with one local representative of each [gauge orbit](../../../../../../gauge-orbit.md). The [Faddeev-Popov gauge-orbit identity](../../../../../../faddeev-popov-gauge-orbit-identity.md) is $1=\Delta_{\mathrm{FP}}[A]\int\mathcal D\omega\,\delta[\mathcal F[A^\omega]]$. Inserting it and factoring out the formal gauge-group volume gives

$$
\boxed{Z=\mathcal N\int\mathcal DA\,\delta[\mathcal F[A]]\det\mathcal M[A]\,e^{iS[A]}.}
$$

The functional delta imposes the gauge condition at every point and for every color. The [determinant](../../../../../../determinant.md) compensates the gauge-orbit Jacobian. For ordinary unoriented real gauge-orbit integration the local Jacobian is $|\det\mathcal M|$; perturbatively its sign is fixed and absorbed into $\mathcal N$, leaving the displayed [determinant](../../../../../../determinant.md). Multiple global intersections, or a [Gribov ambiguity](../../../../../../gribov-ambiguity.md), require more care; the local perturbative formula is not a global uniqueness assertion.

The complex [Grassmann Gaussian integral](../../../../../../grassmann-gaussian-integral.md) now generalizes to spacetime and color indices. Introduce independent anticommuting [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md) $c^a(x),\bar c^a(x)$ and write

$$
\det\mathcal M[A]=\mathcal N'\int\mathcal D\bar c\,\mathcal Dc\,\exp\left(i\int d^dx\,d^dy\,\bar c^a(x)\mathcal M^{ab}[A](x,y)c^b(y)\right).
$$

The factors $i$ in the [functional determinant](../../../../../../functional-determinant.md) differ from a real exponential only by a regulated, field-independent constant. These [Grassmann fields](../../../../../../grassmann-field.md) are Lorentz scalars in the adjoint color representation; the antighost is independent of the ghost rather than an ordinary complex-conjugate commuting variable. They are unphysical fields, not external observable particles. Representing the [functional determinant](../../../../../../functional-determinant.md) by a local ghost [action](../../../../../../action.md) when $\mathcal F$ is local makes ordinary [Feynman rules](../../../../../../feynman-rule.md) available. Anticommutation gives the minus sign of a closed ghost loop, enabling cancellation of unphysical gauge contributions and maintaining the gauge identities in perturbation theory.

For example, the linear covariant choice $\mathcal F^a=\partial^\mu A_\mu^a$ gives $\mathcal M^{ab}=\partial^\mu D_\mu^{ab}$, so non-abelian ghost-gauge interactions remain. In an [axial gauge](../../../../../../axial-gauge.md) $\mathcal F^a=n^\mu A_\mu^a$ with constant $n$, however,

$$
\mathcal M^{ab}=\delta^{ab}n\cdot\partial+gf^{acb}n\cdot A^c\quad\longrightarrow\quad\delta^{ab}n\cdot\partial
$$

on the exact gauge slice. Its [determinant](../../../../../../determinant.md) is field-independent, so **axial-gauge ghosts decouple** and contribute only a normalization factor. This statement uses the strict delta-functional constraint; a finite-width Gaussian gauge weight is not the same exact slice.

The disadvantage is that choosing $n$ obscures manifest Lorentz covariance and the [axial-gauge propagator](../../../../../../axial-gauge-propagator.md) contains spurious $1/(n\cdot k)$ poles. An [axial-gauge pole prescription](../../../../../../axial-gauge-pole-prescription.md) and control of residual transformations satisfying $n\cdot\partial\omega=0$ are necessary; formal decoupling alone does not fix those problems.

**Abelian ghosts do not always decouple.** In a field-independent linear [Lorenz gauge](../../../../../../lorenz-gauge-condition.md), $\delta A_\mu=\partial_\mu\omega$ gives $\mathcal M=\Box$ and they are free. But the [quadratic Abelian gauge fixing](../../../../../../quadratic-abelian-gauge-fixing.md) $\mathcal F[A]=\partial\cdot A+\kappa A_\mu A^\mu$ gives

$$
\delta\mathcal F=(\Box+2\kappa A^\mu\partial_\mu)\omega.
$$

Its [Faddeev-Popov operator](../../../../../../faddeev-popov-operator.md) depends on $A$, and the ghost [action](../../../../../../action.md) contains $2\kappa\bar c A^\mu\partial_\mu c$. This is an explicit abelian ghost-gauge interaction. Abelianity removes the commutator term in the [gauge transformation](../../../../../../gauge-transformation.md), not the field dependence of an arbitrary nonlinear gauge condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
