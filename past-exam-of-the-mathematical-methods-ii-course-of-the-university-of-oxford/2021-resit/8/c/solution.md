<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Away from the origin, write $\mathbf F=r^{-\beta-1}\mathbf r$. The [curl product rule for a scalar field](../../../../curl-product-rule-for-a-scalar-field.md) and the [gradient](../../../../gradient.md) of a radial function give

$$
\nabla\times\mathbf F
=\nabla(r^{-\beta-1})\times\mathbf r
+r^{-\beta-1}\nabla\times\mathbf r
=-(\beta+1)r^{-\beta-3}\mathbf r\times\mathbf r=0.
$$

Consequently the [surface integral](../../../../surface-integral.md) of [curl](../../../../curl.md) over the upper hemisphere is zero. Its outward [unit normal vector](../../../../unit-normal.md) induces a counterclockwise equator when viewed from above. Parametrize that boundary by

$$
\mathbf r(\phi)=r_2(\cos\phi,\sin\phi,0),\qquad
d\mathbf r=r_2(-\sin\phi,\cos\phi,0)\,d\phi.
$$

The radial [vector field](../../../../vector-field.md) is perpendicular to this tangent, so

$$
\boxed{\oint_{\partial S}\mathbf F\cdot d\mathbf r=0
=\iint_S(\nabla\times\mathbf F)\cdot\hat{\mathbf n}\,dS.}
$$

This verifies [Stokes theorem](../../../../stokes-theorem.md) directly without passing through the singular origin.

## ↑ Ancestors (12)

1. [C](../c.md)
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
