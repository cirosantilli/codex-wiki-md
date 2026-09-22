<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an oriented piecewise smooth [surface](../../../../topological-surface-split.md) $S$ with boundary $\partial S$, and a [vector field](../../../../vector-field.md) $F$ continuously differentiable on a neighborhood of $S$, [Stokes theorem](../../../../stokes-theorem.md) states

$$
\boxed{\int_S(\nabla\times F)\cdot n\,dS=\oint_{\partial S}F\cdot dr.}
$$

Here $n$ is the chosen unit [normal vector](../../../../normal-vector.md), $dS$ is the unsigned [surface area element](../../../../surface-area-element.md), and $dr$ is the tangent displacement along the boundary. The [right-hand rule](../../../../right-hand-rule.md) pairs the boundary orientation with $n$. If there are several boundary components, the [line integral](../../../../line-integral.md) includes all of them with their induced orientations.

A [simply connected](../../../../simply-connected-space.md) [surface](../../../../topological-surface-split.md) is connected and every closed loop on it can be continuously contracted to a point while remaining on the [surface](../../../../topological-surface-split.md). A disc is an example. An annulus is not [simply connected](../../../../simply-connected-space.md): a loop winding once around its hole cannot contract within it.

**Stokes' theorem is valid for both types of surface**, under the smoothness and orientation hypotheses above. Simple connectivity is not a requirement of the theorem. For a concrete annular example, take $F=(-y/2,x/2,0)$ and $a\leq r\leq R$ in the horizontal plane. Its [curl](../../../../curl.md) is $(0,0,1)$, so the left side is $\pi(R^2-a^2)$. The right side is the counterclockwise outer-circle integral $\pi R^2$ minus the counterclockwise inner-circle integral $\pi a^2$, giving exactly the same answer. Omitting the inner boundary would be an incorrect application of the theorem.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
