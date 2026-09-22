<h1 id="9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S$ be a compact piecewise smooth [oriented surface](../../../../oriented-surface.md), $\mathbf n$ its chosen unit [normal vector](../../../../normal-vector.md), and $\partial S$ its entire oriented boundary. Let $\mathbf A$ be a continuously differentiable [vector field](../../../../vector-field.md) on a neighborhood of $S$. [Stokes theorem](../../../../stokes-theorem.md) states

$$
\boxed{\iint_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS=\oint_{\partial S}\mathbf A\cdot d\mathbf r.}
$$

Here $\nabla\times\mathbf A$ is the [curl](../../../../curl.md), $dS$ is the [surface area element](../../../../surface-area-element.md), and $d\mathbf r$ is the directed [line integral](../../../../line-integral.md) element. The boundary follows the [right-hand rule](../../../../right-hand-rule.md) relative to $\mathbf n$; equivalently the surface lies to the left when walking along its boundary with one's head toward $\mathbf n$.

The topological requirement is [orientability](../../../../orientability.md), together with the regularity and boundary assumptions above. **Simple connectivity is unnecessary.** An annulus or cylindrical side is allowed, provided every boundary component is included with its induced direction. For a concrete counterexample to a disk-only restriction, take the planar annulus $1\le x^2+y^2\le4$ and $\mathbf A=(-y/2,x/2,0)$. The [curl](../../../../curl.md) is $\mathbf e_z$, the [surface integral](../../../../surface-integral.md) is $3\pi$, and the outer counterclockwise and inner clockwise [line integrals](../../../../line-integral.md) sum to $4\pi-\pi=3\pi$.

For $S$ in the $xy$ [plane](../../../../plane.md) with upward [normal vector](../../../../normal-vector.md) and $\mathbf A=(P,Q,0)$, its [curl](../../../../curl.md) has vertical component $Q_x-P_y$. Thus [Stokes theorem](../../../../stokes-theorem.md) becomes [Green's theorem](../../../../green-theorem.md):

$$
\boxed{\oint_{\partial D}(P\,dx+Q\,dy)=\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)dx\,dy.}
$$

The outer boundary is counterclockwise and any inner boundaries are clockwise.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [9](../../9.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
