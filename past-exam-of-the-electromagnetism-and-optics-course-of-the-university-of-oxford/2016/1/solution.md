<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a contractible region, the [Maxwell equations](../../../maxwell-equations-split.md) $\nabla\cdot\mathbf B=0$ and the [Poincaré lemma](../../../poincare-lemma.md) imply the existence of a [magnetic vector potential](../../../magnetic-vector-potential.md) $\mathbf A$ such that $\mathbf B=\nabla\times\mathbf A$. [Faraday's law of induction](../../../faraday-s-law-of-induction.md) then gives

$$
\nabla\times\left(\mathbf E+\partial_t\mathbf A\right)=0.
$$

The expression in parentheses is a [gradient](../../../gradient.md) there, so a scalar [electric potential](../../../electric-potential.md) $\phi$ can be chosen with

$$
\boxed{\mathbf B=\nabla\times\mathbf A,\qquad \mathbf E=-\nabla\phi-\partial_t\mathbf A.}
$$

These statements are local, or global when the domain has the required topology and the [electromagnetic fields](../../../electromagnetic-field.md) are regular. A nonzero flux through a topologically nontrivial closed surface can obstruct a single globally defined [vector potential](../../../vector-potential.md), even though local expressions remain valid. The [electric potential](../../../electric-potential.md) and [magnetic vector potential](../../../magnetic-vector-potential.md) are not unique: $\mathbf A\mapsto\mathbf A+\nabla\chi$ and $\phi\mapsto\phi-\partial_t\chi$ leave both [electromagnetic fields](../../../electromagnetic-field.md) unchanged.

For the [Lorenz gauge condition](../../../lorenz-gauge-condition.md) $\nabla\cdot\mathbf A=-c^{-2}\partial_t\phi$, [Gauss's law](../../../gauss-s-law.md) becomes

$$
-\nabla^2\phi-\partial_t(\nabla\cdot\mathbf A)=\frac{\rho}{\epsilon_0},\qquad
\left(\nabla^2-\frac1{c^2}\partial_t^2\right)\phi=-\frac{\rho}{\epsilon_0}.
$$

The [Ampere-Maxwell law](../../../ampere-s-circuital-law.md) gives

$$
\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A
=\mu_0\mathbf J-\frac1{c^2}\nabla\partial_t\phi-\frac1{c^2}\partial_t^2\mathbf A.
$$

Cancel the two [gradient](../../../gradient.md) terms using the [Lorenz gauge condition](../../../lorenz-gauge-condition.md). Hence

$$
\boxed{\left(\nabla^2-\frac1{c^2}\partial_t^2\right)\phi=-\frac{\rho}{\epsilon_0},\qquad
\left(\nabla^2-\frac1{c^2}\partial_t^2\right)\mathbf A=-\mu_0\mathbf J.}
$$

Both potential equations have the same [d'Alembert operator](../../../d-alembert-operator.md), with their respective [charge density](../../../charge-density.md) and [current density](../../../current-density.md) sources. In a source-free region these are homogeneous [wave equations](../../../wave-equation-split.md) with propagation speed $c$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2016](../../2016-split.md)
3. [Past exam of the electromagnetism and optics course of the University of Oxford](../../split.md)
4. [Electromagnetism and optics course of the University of Oxford](../../../electromagnetism-and-optics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
