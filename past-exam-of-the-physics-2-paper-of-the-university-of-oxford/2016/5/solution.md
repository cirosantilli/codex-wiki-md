<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The magnetostatic [Ampère's law](../../../ampere-s-circuital-law.md), in vacuum, is

$$
\boxed{\oint_{\partial S}\mathbf B\cdot d\boldsymbol\ell=\mu_0I_{\rm enc},\qquad\nabla\times\mathbf B=\mu_0\mathbf J}.
$$

The path direction and surface normal are related by the right-hand rule. Taking the [divergence](../../../divergence.md) of the differential law gives $\nabla\cdot\mathbf J=0$, since the [divergence](../../../divergence.md) of a [curl](../../../curl.md) vanishes. However, [charge conservation](../../../charge-conservation.md) requires the [continuity equation](../../../continuity-equation.md) $\nabla\cdot\mathbf J=-\partial\rho/\partial t$, which need not vanish during charging.

Using [Gauss's law](../../../gauss-s-law.md), $\nabla\cdot\mathbf E=\rho/\epsilon_0$, the combination $\mathbf J+\epsilon_0\partial\mathbf E/\partial t$ has zero [divergence](../../../divergence.md). Replacing $\mathbf J$ by this conserved total current density gives the [Ampère-Maxwell equation](../../../ampere-s-circuital-law.md):

$$
\boxed{\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t}}.
$$

Its integral form is $\oint\mathbf B\cdot d\boldsymbol\ell=\mu_0[I_{\rm enc}+\epsilon_0\,d\Phi_E/dt]$. The extra term is the [displacement current](../../../displacement-current.md). In a charging parallel-plate [capacitor](../../../capacitor.md), a surface cutting the wire encloses a conduction current $dQ/dt$, while a surface through the vacuum gap encloses no conduction current but has $\epsilon_0d\Phi_E/dt=dQ/dt$. This modification makes the magnetic circulation independent of which spanning surface is chosen. The vacuum [displacement current](../../../displacement-current.md) represents a changing [electric field](../../../electric-field-split.md), not literal transport of charge across the gap.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
