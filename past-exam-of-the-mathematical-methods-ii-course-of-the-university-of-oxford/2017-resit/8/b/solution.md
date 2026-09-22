<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To obtain the [volume integral of a curl](../../../../volume-integral-of-a-curl.md), test its components with an arbitrary constant vector $c$. By part (a), $\nabla\cdot(G\times c)=c\cdot(\nabla\times G)$. Applying the [divergence theorem](../../../../divergence-theorem.md) to the closed boundary, with outward [unit normal](../../../../unit-normal.md) $n$, gives

$$
c\cdot\iiint_V\nabla\times G\,dV
=\iint_S(G\times c)\cdot n\,dS
=c\cdot\iint_S n\times G\,dS.
$$

The last step is cyclic symmetry of the [scalar triple product](../../../../scalar-triple-product.md). Since this holds for every $c$, all vector components agree:

$$
\boxed{\iiint_V\nabla\times G\,dV=\iint_Sn\times G\,dS.}
$$

The same regularity conditions as the [divergence theorem](../../../../divergence-theorem.md) apply: for example a continuously differentiable field on a neighbourhood of a bounded volume with piecewise smooth boundary.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
