<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a continuously differentiable [vector field](../../../../vector-field.md) $\mathbf F$ on a neighborhood of an oriented, piecewise smooth [surface](../../../../topological-surface-split.md) $S$, [Stokes theorem](../../../../stokes-theorem.md) states

$$
\boxed{\oint_{\partial S}\mathbf F\cdot d\mathbf r
=\iint_S(\nabla\times\mathbf F)\cdot\hat{\mathbf n}\,dS.}
$$

Here $\partial S$ is the boundary [curve](../../../../curve.md), $d\mathbf r$ is its directed tangent element, $\hat{\mathbf n}$ is the chosen [unit normal vector](../../../../unit-normal.md), $dS$ is the [surface area element](../../../../surface-area-element.md), and $\nabla\times\mathbf F$ is the [curl](../../../../curl.md). The [right-hand rule](../../../../right-hand-rule.md) relates the boundary direction to $\hat{\mathbf n}$. Thus [circulation](../../../../circulation-physics.md) around the edge equals the [flux](../../../../flux.md) of [curl](../../../../curl.md) through the spanning [surface](../../../../topological-surface-split.md). Reversing both orientations changes both signs. One can replace a difficult [line integral](../../../../line-integral.md) by an easier [surface integral](../../../../surface-integral.md), or replace one spanning [surface](../../../../topological-surface-split.md) by another within the region of regularity.

For a bounded [volume](../../../../volume.md) $V$ with piecewise smooth closed boundary and a continuously differentiable [vector field](../../../../vector-field.md) on a neighborhood of its closure, the [divergence theorem](../../../../divergence-theorem.md) states

$$
\boxed{\iint_{\partial V}\mathbf F\cdot\hat{\mathbf n}_{\rm out}\,dS
=\iiint_V\nabla\cdot\mathbf F\,dV.}
$$

Here $\hat{\mathbf n}_{\rm out}$ points out of $V$, including into any holes, $dV$ is the [volume element](../../../../volume-element.md), and $\nabla\cdot\mathbf F$ is the [divergence](../../../../divergence.md). It equates total outward [flux](../../../../flux.md) to integrated source strength. It converts a closed [surface integral](../../../../surface-integral.md) into a [volume integral](../../../../volume-integral.md), and explains why internal [fluxes](../../../../flux.md) cancel in a subdivided region. Singularities cannot be included without checking the hypotheses.

For a [conservative force](../../../../conservative-force.md), the [work](../../../../work.md) around every closed path is zero. [Stokes theorem](../../../../stokes-theorem.md) gives zero [flux](../../../../flux.md) of [curl](../../../../curl.md) through every sufficiently small patch. Dividing by its area and shrinking the patch shows that every component of the continuous [curl](../../../../curl.md) vanishes:

$$
\boxed{\oint_C\mathbf F\cdot d\mathbf r=0,\qquad
\nabla\times\mathbf F=0,\qquad \mathbf F=-\nabla U.}
$$

Here $U$ is [potential energy](../../../../potential-energy.md); conversely, zero [curl](../../../../curl.md) implies a [conservative vector field](../../../../conservative-vector-field.md) on a [simply connected domain](../../../../simply-connected-domain.md). The [divergence theorem](../../../../divergence-theorem.md) then gives the compatible relation $\iint_{\partial V}\mathbf F\cdot\hat{\mathbf n}\,dS=-\iiint_V\nabla^2U\,dV$. There is no general zero-[divergence](../../../../divergence.md) condition on a [conservative force](../../../../conservative-force.md): $\mathbf F=-\mathbf r=-\nabla(r^2/2)$ is a concrete counterexample, with $\nabla\cdot\mathbf F=-3$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
