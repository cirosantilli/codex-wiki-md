<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Stokes theorem](../../../stokes-theorem.md) gives $\int_S(\nabla\times\mathbf F)\cdot\hat{\mathbf n}\,dS=\oint_{\partial S}\mathbf F\cdot d\mathbf r$ for a sufficiently smooth [vector field](../../../vector-field.md) and consistently oriented [surface](../../../topological-surface-split.md) and boundary. Choose the hemisphere's outward [normal vector](../../../normal-vector.md); its boundary circle is then traversed counterclockwise viewed from $+z$. Parametrize it by $\mathbf r=(2\cos t,2\sin t,0)$, $0\leq t\leq2\pi$. On this curve, $\mathbf F=(8\sin t,2\cos t,0)$ and $d\mathbf r=(-2\sin t,2\cos t,0)dt$. Therefore

$$
\boxed{I=\int_0^{2\pi}(-16\sin^2t+4\cos^2t)dt=-12\pi.}
$$

As a check, $\nabla\times\mathbf F=-3\hat{\mathbf z}$, whose flux is $-3$ times the projected disk area $4\pi$, not $-3$ times the hemisphere's surface area. Reversing orientation gives $+12\pi$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2014](../../2014-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
